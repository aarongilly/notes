---
tags:
- modeling
---
**Ports function like “tunnels” in [[IDEF0]].**

Per VisualParadigm’s online training, at **least** when it comes to [[Component Diagrams]]:

> A port (definition) indicates that the component itself does not provide the required interfaces (e.g., required or provided). Instead, the component delegates the interface(s) to an internal class.
> 

![Untitled](Untitled%2030.png)

So, in this case, the `IdentityManagement` interface provided by the `Member Management` component is *actually* provided by an **internal class** within `Member Management`.
### Source
- [Component Diagram Tutorial](https://online.visual-paradigm.com/diagrams/tutorials/component-diagram-tutorial/)

### Related Notes
- [[Component Diagrams]]