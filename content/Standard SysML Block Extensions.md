---
created: 2023-07-08
aliases: 
tags:
  - modeling
---
**Actor, Constraint, Interface, Value Type, Enum**

Blocks function like Classes in object-oriented coding languages. In this metaphor, the most generic class is simply `Block`. SysML enables you to create your own custom extensions of Blocks, but also provides many standard ones out of the box. All blocks contain a `name`.

This is an incomplete list.

## Actor

Represents an agent. Has no other special properties.

### Constraint

Represents a constraint that can be bound to other blocks. 

Contains a constraint `expression`, and constraint `parameters`.

### Interface

Represents a behavioral contract that can be used to decouple blocks from their relationships. They describe what configurations the block can receive or provide.

Contains `operations` and `receptions`.

### ValueType

Represents a type of value that a can be reused to type block properties. For example, you may have a ValueType for DateTime. SysML comes pre-built with a library of base ValueTypes.

May contain additional `values` elements, if the ValueType represents a [[Tuple]].

### Enumeration

Represents a bound set of values that a can be used to type properties. Similar to ValueType, but with a more specific use case. An Enumeration could be built to type a DayOfWeek property, where the only values are [’monday’, ‘tuesday’, .... ‘sunday’].

Contains the enumeration `Literals`.

---

### Source
- [[SysML Distilled]]

### Related
- [[SysML Blocks]] 
- [[Tuple]] 
- [[SysML Block Property Types]]