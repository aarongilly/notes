---
created: 2023-07-08
aliases: 
tags:
  - modeling
---
**IDEF Process Description Capture.**

IDEF3 is a method for capturing and documenting processes. Like the other IDEF methods, it’s primarily graphical in nature - but also specifies a textual representation. IDEF3 diagrams come in three varieties:

**Process Schematics** are akin to [[SysML]] [[Activity Diagrams]].

**Object Schematics** are akin to SysML [[Block Definition Diagram ]].

**Transition Schematics** are akin to SysML [[State Diagrams]], or [[OPM]] diagrams.

IDEF3 also specifies an **Elaboration Language**, which is a formal means of describing models using textual representation. There’s zero reason to ever learn it, and its syntax looks unapproachable to a layperson.

Like most modeling techniques, IDEF3 supports [[Decomposition Understanding]]. You can “zoom in” to greater levels of fidelity, or “zoom out” to greater levels of scope.

![Untitled](Untitled%2054.png)

## Process Schematics

![Untitled](Untitled%2055.png)

Process Schematics describe processes. Above is an example of a process schematic. The fundamental unit of a Process Schematic is a ‘**unit of behavior**’ (UOB), which is a self-contained real-world process, individually labeled and indexed. The UOBs are connected via links, which may flow through aggregation points (AND, OR, XOR). They are indexed with a unique key, which can be used to positively identify any given UOB for unambiguous reference elsewhere (typically for elaboration).

![Untitled](Untitled%2056.png)

## Object Schematics

![Untitled](Untitled%2057.png)

Object Schematics describe objects. They are composed of each other, linked together via transition links or labeled relationship links, and may be stateful. IDEF defines first-order relations as relations between objects themselves, and 2nd order relations as relations between the *types* of objects. 

![Untitled](Untitled%2058.png)

## Transition Schematic

![Untitled](Untitled%2059.png)

The real power of IDEF3 is when Process and Object Schematics collide. A Transition Schematic describes how Processes and Objects inter-relate. They can *also* contain sections that are process-specific and sections that are object-specific. 

### Elaboration Language

It’s there, so I’m including it. Don’t worry about it, though. I cannot imagine it’s in use in any real way today. Also it looks like this:

```
(forall (?coe : (activation-of ?coe PQD))
(forall (?sit : (and (occurs-in ?sit ?coe) (occurrence-of ?sit Paint-part)))
(not (exists-5 ?x (and (instance-of ?x Part)
(supports ?sit (in-queue ?x Q (start-of ?sit) +))))))
```

****
### Source

[IDEF3 - Process Description Capture Method - IDEF](https://www.idef.com/idef3-process-description-capture-method/)

### Related
- [[IDEF]] 
- [[IDEF5]] 
- [[Activity Diagrams]] 
- [[State Diagrams]] 
- [[Block Definition Diagram ]]
- [[Diagram Types (index)]]