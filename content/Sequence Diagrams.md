---
aliases: 
tags:
  - coding
  - modeling
---
**A tool for displaying how interactions between participants occur - very useful for software & process development.**

Sequence diagrams depict a sequence of activities, arranged sequentially along the vertical access, between two or more participants (which may be people, systems, or objects). The lines flowing between the participants carry text describing that portion of the interaction, this is often called ‘messaging’ in this context. The primary value proposition for these types of diagrams is in relating the constraints in *sequencing* of these messages. **Lifelines** are the boxes along the vertical axis that shows when participants are engaged in the sequencing process.

I’ve found Sequence Diagrams very helpful when designing simple systems.

## Example

From my actual use of this...

```mermaid
sequenceDiagram
    autonumber 
    participant dbHost
    participant apiHost
    actor client
    Note over client: Search for Entries
    client-->>apiHost: query string
    apiHost-->apiHost: parse request 
    alt is invalid
    apiHost-->client: bad query
    else is valid
    apiHost-->>dbHost: xlated query
    dbHost-->dbHost: fetch results
    dbHost-->>apiHost: raw data
    apiHost-->apiHost: perform shaping
    apiHost-->>client: results
    end
```

---

### Source


### Related
- [[UML]] / [[SysML]]