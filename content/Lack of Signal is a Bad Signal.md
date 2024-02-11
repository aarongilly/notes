---
created: 2023-07-08
aliases: 
tags:
  - technique
  - coding
  - modeling
  - systemdesign
---
**When designing a system, don’t use e.g. “lack of yes” as the “no” condition.**

When designing a system, avoid utilizing the “lack of signal received” as an indicator. It is a much more robust practice to give clear and explicit signals that NECESSARILY MUST have been created intentionally than it is to utilize some implicit signal like “well, he didn’t tell me there was an issue so I assume it’s fine”. 

This can be manifest in writing an API or a sufficiently complicated function returning an object. Tack on a “status” flag with the resultant, and have it set explicitly.

Utilizing a Lack of Signal as a signal is an [[Error Trap]].

---

### Source

### Related
- [[Error Trap]]