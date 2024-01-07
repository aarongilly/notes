---
tags:
  - coding
  - data
created: 2023-07-08T11:37-05:00
updated: 2023-08-11T11:23-05:00
---
**A JSON shape description language, using JSON**

JSON is inherently schema-less. It’s not relational. It’s not the kind of structure that makes up the “S” in “SQL”. It’s more free-form. It’s nested.

Sometimes, however, there’s a need to constrain (or just *describe*) what shapes a particular use of JSON are allowed to take. JSON Schema is a IETF Standard & language (with specification) for doing just that.

JSON Schema is used in the [[OpenAPI]] standard, as well.

## Example

### JSON

```jsx
{
  "id": 7,
  "name": "John Doe",
  "age": 22,
  "hobbies": {
        "indoor": [
            "Chess"
        ],
        "outdoor": [
            "BasketballStand-up Comedy"
        ]
    }
}
```

### JSON Schema

```jsx
{
    "$schema": "http://json-schema.org/draft-04/schema#",
    "$id": "https://example.com/employee.schema.json",
    "title": "Record of employee",
    "description": "This document records the details of an employee",
    "type": "object",
    "properties": {
        "id": {
            "description": "A unique identifier for an employee",
            "type": "number"
        },
        "name": {
            "description": "Full name of the employee",
            "type": "string"
        },
        "age": {
            "description": "Age of the employee",
            "type": "number"
        },
        "hobbies": {
            "description": "Hobbies of the employee",
            "type": "object",
            "properties": {
                "indoor": {
                    "type": "array",
                    "items": {
                        "description": "List of indoor hobbies",
                        "type": "string"
                    }
                },
                "outdoor": {
                    "type": "array",
                    "items": {
                        "description": "List of outdoor hobbies",
                        "type": "string"
                    }
                }
            }
        }
    }
}
```

---

### Source
- [JSON Schema Examples Tutorial](https://www.mongodb.com/basics/json-schema-examples)
- [JSON Schema](https://json-schema.org/)

### Related Notes
- [[JSON]]