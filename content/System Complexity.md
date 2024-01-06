---
tags:
  - systemdesign
summary: A hard thing to define, has many parts - ironically
aliases:
  - complex systems
---
**`= this.summary`**

"Complexity" is hard to define. It is somewhat subjective, but also things can be objectively complex. The best definition of complexity would be something like:

> [!tldr] Complexity
> The degree to which it is difficult to understand how a system will operate, and predict the consequences of changing it. 
> The degree to which it is difficult to predict the properties of a system if the properties of its parts are given.

It is difficult to predict or determine the state of a *complex* system given a view of one of its constituent parts. Complex systems don't have a clear relationship between its elements do and what the system as a whole does. This can be due to unclear constraints, rules, hidden dependencies, and [[Emergent Behavior]].

Complexity can be *disorganized* or *organized*. Weirdly those things are sort of backwards from what you figured they'd mean. Organized complexity is *harder* to analyze using statistical techniques.

## Objective Complexity
Some complexity is objective, where it is not possible (by anyone with any amount of knowledge) to predict a system's behavior given its current state & history.  Elements of Objective complexity include:
1. **Independence** - the ability of components of a system to make their own decisions based on inputs from other systemic components or the environment
2. **Interconnectedness** - how interdependent the components of the system are
3. **Diversity** - how intrinsically different the aspects of the system are
4. **Adaptability** - the responsiveness to change of a components behavior based on circumstances, may be due to humans-in-the-loop or software

## Subjective Complexity
More worth considering, though, is *subjective complexity*. That is, how quickly and easily can the layperson understand the system and predict what it's going to do next. An expert (e.g. the system designer) could perhaps perfectly predict what's going to happen, but it's non-obvious to a casual observer. This is subjective complexity, and it causes failures of adoption. This is a matter of perspective, and *must be considered* when design systems. 

[[Affordances]] and piggybacking on [[Standard Processes]] lessen subjective complexity.



---
### Source
- [[Systems Engineering Book of Knowledge]]

### Related
- [[Systems Engineering]]
- [[What is a System]]