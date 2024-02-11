---
created: 2023-07-08
aliases: 
tags:
  - modeling
---
**A business architecture Modeling language**

Archimate is an ‘Open’ modeling language aimed at representing enterprise architecture. It’s a single-diagram-type visual language, very similar to my own ideas. Multiple “Views” exist representing the same fundamental model in accordance with different perspectives. It uses node colors, shapes, and symbols to signify the types of elements and their essence.

It was build by “The Open Group”, which means its related to TOGAF (The Open Group Architecture Framework).

Its scope is intended to be limited to [[Enterprise Architecture]]. The language does **not** include some constructs that would be helpful in other domains (e.g. data modeling). You can't, for example, define a multiplicity on a Composition Relationship.

## Core Framework

Archimate “core” framework covers the Subjects, Behaviors, and Objects in a business across 3 “layers” - business, application, and technology.

![https://www.visual-paradigm.com/guide/archimate/what-is-archimate/](https://www.visual-paradigm.com/servlet/editor-content/guide/archimate/what-is-archimate/sites/7/2018/05/02-archimate-core-framework.png)

From [https://www.visual-paradigm.com/guide/archimate/what-is-archimate/](https://www.visual-paradigm.com/guide/archimate/what-is-archimate/)

Passive Structure is like the subject of a sentence, the behavior is the verb, the active structure is the object. “Computer Serves Ticket” is an example of each in sentence form.

The “Layers” don’t seem all that useful. They are organized in accordance with “services” and what realizes those services. The business runs on applications. The applications run on technologies.

## Full Framework

![full framework](https://www.visual-paradigm.com/servlet/editor-content/guide/archimate/what-is-archimate/sites/7/2018/05/05-archimate-full-framework.png)

From [https://www.visual-paradigm.com/guide/archimate/what-is-archimate/](https://www.visual-paradigm.com/guide/archimate/what-is-archimate/)

The ‘full’ framework adds a few more layers, and a special “Motivation” extension which includes requirements, goals, principles, and drivers.

#### Full Metamodel
This is very helpful.
![good graphic.](https://www.hosiaisluoma.fi/blog/wp-content/uploads/2018/09/Metamodel-3.1-full-1.png)

## Views & Viewpoints

There are a bunch (but notably much fewer than [[UAF]]) of standard viewpoints that are suggested by the markers of Archimate. Each of the views is associated with some subset of model element types and relationship types. Each is meant to illustrate some particular part of the architecture. 
#### Example: application usage viewpoint.
![Application Usage Viewpoint Example](https://cdn-images.visual-paradigm.com/guide/archimate/full-archimate-viewpoints-guide/05-archimate-application-usage-viewpoint.png)

In the example viewpoint, the constructs are limited to application components, which realize (dotted line with open triangle connector) services, which serve (basic arrow) functions.
## Software

There are multiple softwares that support Archimate. The ‘official’ version is the Open Source “[Archi](https://www.archimatetool.com)”, which is pretty good.

---

### Source
- [Visual Paradigm: What is ArchiMate?](https://www.visual-paradigm.com/guide/archimate/what-is-archimate/)
- [The ArchiMate® Enterprise Architecture Modeling Language](https://www.opengroup.org/archimate-forum/archimate-overview)
- [A great example page](https://gbruneau.github.io/ArchiMate/)

### Related
- [[SysML]] 
- [[OPM]] 
- [[MBSE]]