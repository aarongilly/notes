---
created: 2023-07-08
aliases: Object Process Methodology
tags:
  - technique
  - clarity
  - modeling
---
**Object-Process Methodology - a bi-modal, single-diagram systems modeling language.**

Object-Process Methodology is a systems modeling language, conceived of in the mid-90's by a guy named Dov Dori, and standardized by the [[ISO]] in 2015 as ISO 19450. The purpose of OPM is to support conceptual design, possibly best even for ***early*** conceptual design. 

Unlike some of its more popular alternatives (see: [[SysML]]) OPM has exactly **one kind of diagram**. This diagram roughly relates to a state diagram in [[UML]]/SysML, but can be utilized to show structure, behavior, use cases, and (to some extent) Sequence Diagrams. 

Like most other modeling techniques, it embraces the idea of levels of decomposition. Its diagrams may be zoomed in and out-zoomed to decompose to your desired level of granularity. 

There is a free tool called OPCAT (which has evolved into [https://www.opcloud.tech](https://www.opcloud.tech/)) for creating OPM models.

OPM is about Objects, which have States, which are created, modified, and consumed by Processes, and the processes that link between them. Processes and Objects are "equal players" in the OPM model. Objects and Processes always come in pairs. A Process doesn't exist without some sort of Object(s) that it modifies. Processes are described using their gerund form ("kicking", not "kick"). Objects are represented with rectangles. Processes with ovals. Arrows between them have different conventions which each have their own assigned meanings. 

OPM is bi-modal - **is it has two modes of existence** (one graphical, and one textual) that can directly translate to one another. These modes are called Object-Process Diagram (OPD) and Object-Process Language (OPL).

The [Wikipedia Article](https://en.wikipedia.org/wiki/Object_Process_Methodology) is *incredibly* thorough. The rabbit hole for [[Ontology, Semantics, and Syntax]] for this language is too deep for here. Here are some of the natively supported concepts:

- Things (objects and processes) have:
    - Name
    - Description
    - Essence - physical or informational
    - Perseverance - is it static or dynamic
    - Affiliation - is it part of the system or part of the environment
- Object States
    - Initial
    - Final
    - Default
- Link types
    - Object-to-Object or Process-to-Process
        - Aggregation/participation
        - Exhibition/characterization
        - Generalization/Specialization
        - Classification/Instantiation
        - Tagged structural links (sort of a generic link) that can be bidirectional with different text in either direction, in a way that's actual intuitive. Nice.
    - Object-to-Process
        - Transforming type
            - Consumption Link
            - Resultant Link
            - Affects Link
        - Enabling type (mechanisms from IDEF)
            - Agent
            - Instrument
        - Control type
            - Event (e)
            - Condition (c)
    - Invocation Link
        - Processes can invoke other processes
        - Processes can invoke themselves
- Relationship Cardinalities

---

### Source
- [Object Process Methodology - Wikipedia](https://en.wikipedia.org/wiki/Object_Process_Methodology)

### Related
- [[Ontology Language]] 
- [[Ontology, Semantics, and Syntax]] 
- [[SysML]] 
- [[UML]]