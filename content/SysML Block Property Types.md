---
tags:
  - modeling
created: 2023-07-08T11:37-05:00
updated: 2023-07-09T10:44-05:00
---
**Part, Reference, Value, Constraint, Port**

Blocks in [[SysML]] (essentially like Classes in [[UML]]) are capable of holding properties of many different types. Including...

## Part Properties

Literally the *parts* of a block. 

Block `Car` has part property `Wheel`

Part properties are typically displayed in the  parts compartment of a block with the syntax

```
<part name> : <type> [<multiplicity>]
```

---

## Source
- [[SysML Distilled]]

## Reference Properties

Reference properties are similar to part properties, in that they imply the block must have the reference property in order to fulfill its function - but it doesn’t imply *ownership* over the block. 

Block `Car` has reference property `Owner`

## Value Properties

Value properties are essentially facts about the block. They are typically numeric with an associated unit of measure (or sometimes string literals).

Block `Car` has value property `Weight` which is measured in `kg`.

These are most typically what constraints are written against. Speaking of which...

## Constraint Properties

These properties are rules that an instance of a block must satisfy to be valid. They are typically represented as mathematical formulas or inequalities on Value Properties.

Block `Car` must have a `Weight` that is `> 0kg`

## Port Properties (or, just ‘ports’)

Port Properties represent distinct interaction points on a block in which signals, energy, or matter can be transmitted. Blocks may have many ports, or no ports. Ports may have requirements about the interfaces they accept or expose. Most typically when interacting with a block, agents know about *port*s and don’t have to know about the inner workings of the system. Thus ports decouple the activity from the implementation.

Block `Car` has port `Gasoline Inlet` in

### Related Notes
- [[Block Definition Diagram ]] 
- [[Standard SysML Block Extensions]] 
- [[SysML Blocks]]