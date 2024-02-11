---
created: 2023-07-08
aliases: 
tags:
  - modeling
---
**A SysML-specific diagram for illustration of requirements and their relationships to everything else.**

Relationship diagrams illustrate the Requirements A system was designed around. It allows you to define relationships of various types between requirements and any other element, such as their parent requirements, verification activities, blocks that satisfy requirements, and associated use cases, to name a few examples. 

## Requirements Blocks

Have an ID & requirement text. Additional properties can exist if you create them (e.g. ‘criticality’).

# Requirements Relationships

There are 6 main relationship types for requirements.

### Containment

Requirements contained in requirements specifications, for example. 

## Trace

A trace relationship says there is a loose dependency between the requirement and the other element. It carries no specific semantic meaning beyond that.

## Derive

A derive relationship is a dependency between requirements pointing from a parent requirement to a more specific requirement that was derived from it.

## Refine

A refine relationship is a dependency between an abstract requirement and something else (often a Use Case) which provides a more a more specific reasons for the requirement.

## Satisfy

A relationship from a requirement to a block that is asserted to satisfy the intent of the requirement.

## Verify

A relationship from a requirement to a test case (which is a behavior modeled using a an Activity, Interaction, or State Machine).

# Example Representations

### Direct Notation

![[90A67798-5728-4699-85DE-0DA421F7CD87.jpeg.jpeg]]

### Compartment Notation

![[CCAA7FAD-DAA5-4521-BC6C-AFCF592D40EB.jpeg.jpeg]]

### Matrix Notation

![[9B6CDD59-425B-45AE-BFB9-AB0E6C1786A8.jpeg.jpeg]]

---

### Source
- [[SysML Distilled]]

### Related
- [[SysML]]