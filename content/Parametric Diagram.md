---
tags:
  - modeling
created: 2023-07-08T11:37-05:00
updated: 2023-07-09T10:44-05:00
---
**A unique SysML diagram used for representing constraints, often through mathematical relations.**

Parametric Diagrams are (along with [[Requirements Diagram]]) unique to [[SysML]] (i.e. not found in [[UML]]). Parametric Diagrams are used to represent system constraints, often through the use of mathematical relations, by binding elements in the system to constraints. They say “this property of this block is bound to that property of that block via this formula”. Parametric Diagrams are what allows SysML to be simulatable.

Constraints have `Constraint Parameters`, which are bound to Block `Value Properties`.

Parametric diagrams are exploded views of Blocks, and sometimes more specifically *Constraint* Blocks. If a parametric diagram is representing a Constraint block, it will have ports along the boundaries of the diagram frame, representing input and output points. Otherwise, if the diagram is representing a more generic block, the diagram may be self-contained.

![[assetsFBD6B2CA-6A72-46A1-83B0-C1B43440CB33.jpeg]]

---

## Source
- [[SysML Distilled]]

### Related Notes
- [[SysML]] 
- [[Standard SysML Block Extensions]]