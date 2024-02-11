---
created: 2023-07-08
aliases: 
tags:
  - coding
  - technique
---
**Major.Minor.Patch, ^=minor, ~=patch**

# Semantic Versioning (SemVer)

The default versioning method in npm. Version numbers mean something!

```json
"package": "MAJOR.MINOR.PATCH"
```

## Definitons

- **MAJOR** - Increment this when making backwards-incompatible API changes
- **MINOR** - Increment this when you add functionality that's backwards-compatible
    - Prefixing dependencies with "^" allows npm to use the most recent MINOR release
- **PATCH** - Increment this when you're doing bugfixes (and bugfixes shall be backwards-compatible)
    - Prefixing dependencies with "~" allows npm to use the most recent PATCH release

---

### Source
- [[freeCodeCamp]]

### Related
- [[NodeJS]]