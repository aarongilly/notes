---
aliases: RDF
tags:
  - data
  - coding
  - modeling
---
**Resource Description Framework:  Subject - Predicate - Object**

RDF is not a Language, it is a method for describing and exchanging graph data. RDF can be serialized by different [[Data Serialization Methods]], one example of which is [[JSON-LD]]. Is is a triple (or quad) store for:

Subject - Predicate - Object (and context)

...using [[URI]]s.

![[AA2E5F3A-4555-4508-B5F4-D9EB9CDDA70B.jpeg.jpeg]]
## Example

```
<http://example.org/person/Mark_Twain>
   <http://example.org/relation/author>
   <http://example.org/books/Huckleberry_Finn> .
```

---

### Source
- [[Wikipedia]]

### Related
- [[Graph Database]] 
- [[Data Serialization Methods]]
- [[JSON-LD]]
- [[URI]]