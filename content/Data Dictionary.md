---
created: 2023-07-08
tags:
  - data
  - systemdesign
  - modeling
aliases:
---
Data Dictionaries are metadata repositories. They don't hold the data, they hold the information that *describe* the data. They are composed of names and descriptions of the various tables of your [[Relational Databases]], and often the relationships between them (like in an [[Entity-Relationship Diagrams]]). Having a data dictionary is a good thing, even better when you can marry them in with [[Data Flow Diagram]]s or other types of [[Diagram Types (index)|Diagrams]].

Data Dictionaries can be *active* or *passive*. Passive data dictionaries are essentially static representations of the database. Active data dictionaries are capable of self-updating on database changes and/or imposing *constraints* on the data stored (e.g. "this `int` field only goes from 0 to 10").
## Typical Attributes
Each field would have associated with these meta-data attributes:
- Group Name
- Name
- Displayed Title
- [[Data Types|Type]]
- Constraints (e.g. max/min, decimal place count)
- Default value
- Prompt type
- Is required
- Is read only
- Is unique
- Event-driven handlers (e.g. "on-click" routines)
- Formatting info
- Description

---
### Source
- [Wikipedia](https://en.wikipedia.org/wiki/Data_dictionary)

### Related
- [[Data Flow Diagram|DFD Diagrams]]