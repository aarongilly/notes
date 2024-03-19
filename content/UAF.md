---
created: 2023-12-18
aliases: 
tags:
  - modeling
  - business
  - technique
summary: Unified Architectural Framework - an Enterprise Architecture modeling solution
---
UAF is by Object Management Group, the people behind [[SysML]]. It's based on SysML and a few other pre-existing [[Enterprise Architecture Frameworks]].

## 72 Views
The UAF table is actually a table of *views*. UAF is basically a superset of NATO and DODAFs frameworks. 

![[IMG_1133.jpeg]]

**Not all 72 views are needed for an EA**. In the video linked below James Martin suggest the ceiling for an expected amount of views represented in an EA is about ~15.

## The 8 Building Blocks
The Standard [[SysML]] "Block" has been refined into a number of different classes.

![[IMG_1134.jpeg]]

## Example Domain 
In the UAF Guide they detail the different domains from the UAF Grid. This is a meta model of on example domain, the Service Domain. This domain is centered around the **service**, which own a port that is typed by an interface. I suspect the color coding is part of the standard, but haven't read it yet. 

![[IMG_1137.jpeg]]

****
### Source
- https://www.omg.org/uaf/
- https://www.omg.org/spec/UAF/1.2/UAFML/PDF - the official Spec
- https://www.omgwiki.org/uaf/lib/exe/fetch.php?media=dtc-21-12-13.pdf - EA Guide for UAF

### Related
- [[SysML]]
- [[Archimate]]