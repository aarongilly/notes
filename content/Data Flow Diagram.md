---
created: 2023-07-08
tags:
  - data
  - systemdesign
  - notetaking
aliases:
  - DFD Diagrams
---
Data Flow Diagrams represent data flows in a graphical way. There is no single *governing body* or "*official*" specification that DFD Diagrams "shall" adhere to. They evolved out of the same "[[IDEF0 and SADT|SADT]]" effort that eventually led to [[IDEF0]], and this share a lot of commonalities. 

![[IMG_5814F855AFF9-1.jpeg]]

Several example diagrams I've found document more than just "data":
![[IMG_D9A0AA5B612D-1.jpeg]]
...which basically just turns a DFD Diagram into [[OPM]] or [[IDEF3]].

There are apparently 2-to-4 main competing syntaxes. 
- Yourdon-Coad 
- Gane-Sarson
- "Unified" - which uses the `<<stereotype>>` notation from [[UML]] & [[SysML]].
## Features
- Like [[IDEF0]]...
	- they are essentially self-explanatory 
	- they are meant to be small & simple, achieved through decomposition and hierarchy
		- Including a top-level "Level 0" diagram, aka "Context Diagram"
	- Don't include mechanisms for control flow & boolean logic
		- It *can* represent situation-dependent flows, though. A function's may have two outputs "`valid phone number`" and "`invalid phone number`", for example.
	- Elements in the diagram are uniquely numbered
- Components[^1]
	- **Data flows** - arrows
	- **Processes** - circles
	- **Data Stores/Entities** - rounded rectangles
		- From a [[Systems Thinking]] perspective, these are "*stocks*"
		- There's an implied semantic meaning for including a "store" instead of just using data flows to connect processes directly to each other, if a store is present, that means it **exists** in some enduring form. It also means the functions write to/read from the store, as opposed to talking directly to one-another.
	- **Terminators/External Entities** - rectangles
- [[Decomposition Understanding]]
	- Diagrams can be defined hierarchically, using the same type of "drill in" rules as found in [[IDEF]] and [[OPM]]

## Complimentary Practices
[[Just Enough Structured Analysis]] suggests DFD Diagrams are *necessary but not sufficient* for representing system behavior. It suggests the need to combine DFD Diagrams with [[Data Dictionary|Data Dictionaries]] and Process Specifications[^2].

[^1]: syntaxes here are dependent on which type, in practice to they sort of come through in their usage

[^2]: Apparently "Process Specification" here can be anything from flowcharts to pseudo code to structured English. 

---
### Source
- [Wikipedia](https://en.wikipedia.org/wiki/Data-flow_diagram)
- [This article](https://blog.hubspot.com/marketing/data-flow-diagram/)
- [[Just Enough Structured Analysis]]

### Related
- [[IDEF0]]
- [[RAS Syndrome]]