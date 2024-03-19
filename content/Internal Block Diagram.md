---
created: 2023-07-08
aliases: 
tags:
  - modeling
---
**Represent the internal structure of a SysML Block.**

Internal Block Diagrams (IBD) allow for the elaboration on a given [[SysML Blocks]]. Each IBD is bound to and represents a particular Block. It explains more information about valid configurations block instances have to uphold. The are used to convey:

- Show Block Reference Properties bound to the things they reference.
- Connectors between properties internal to the block
- Connectors to outside elements, via ports
- The types of matter/information (’Item Flows’) that are associated with these connections

IBDs are contextualized by [[Block Definition Diagram ]]s. It’s a common practice in [[SysML]] to have a tick-tock approach wherein BDDs and IBDs are used in an alternating fashion to “zoom in” on particular aspects of a system (enabling [[Decomposition Understanding]]).

See how BDDs contextualize IBDs.

![Examples borrowed from ‘A Practical Guide to SysML’](Untitled%2033.png)

Examples borrowed from ‘A Practical Guide to SysML’

****
### Source
- [[SysML Distilled]]
- A Practical Guide to SysML - book

### Related
- [[SysML]] 
- [[SysML Blocks]] 
- [[Block Definition Diagram ]] 
- [[Decomposition Understanding]]