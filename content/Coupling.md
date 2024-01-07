---
created: 2023-07-17T14:47-05:00
updated: 2023-07-17T15:24-05:00
---

**The extent to which two components depend on each other for successful execution.** 

Coupling is a thing that happens *between* system components. Unlike [[Cohesion]], Coupling is **inter-component**.

Coupling is something that sometimes cannot be avoided, but when it **can** be avoided, it should be. High levels of coupling reduces a system's [[Modularity]], or at the very least makes module-level changes more complex due to inter-module dependencies.

Coupling should be managed via well-defined, well-managed, well-though-out, and well-documented interfaces.

In general, **low-coupling is good**.

### Example of High-Coupling
- Including presentation features inside a data source table

### Examples of Low-Coupling
- A source data table and a table for how a particular view should be formatted

---
### Source
- [[Udacity Software Architecture Course]]

### Related
- [[Highly Cohesive, Loosely Coupled]]

#### Tags
#modeling #coding #systemdesign 