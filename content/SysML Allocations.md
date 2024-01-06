---
tags:
- modeling
---
**A versatile relationship with no specific meaning.**

Allocations are a generic type of relationship that can exist between any two kinds of elements, and used however you (the modeler) see fit. Despite not being defined in the spec, allocations have some typical uses. b

### Allocating Requirements to Structures

```mermaid
flowchart LR
a(Req: system shall be able to store 100gb) --allocate--> b(2.5in HDD Drive)
```

### Allocating Behaviors to Structures

```mermaid
flowchart LR
a(load file) --allocate--> b(2.5 HDD Drive)
```

### Allocation Logical Structures to Physical Structures

```mermaid
flowchart LR
a(cold storage) --allocate--> b(2.5in HDD Drive)
```

---

### Source
- [[SysML Distilled]]

### Related Notes
- [[Requirements Diagram]] 
- [[Block Definition Diagram ]] 
- [[Internal Block Diagram]] 
- [[SysML]]