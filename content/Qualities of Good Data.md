---
created: 2024-02-06
tags:
  - business
  - data
  - manufacturing
aliases:
---
Data is the new gold... but data (outside of the types of machine learning systems used to train [[Large Language Models]]) needs a few things to be *useful*.

This list is from my own mind. There are probably more authoritative sources that would suggest a better set of principles.

Good data is:
- **Discoverable & accessible** - you can't use what you don't know exists or can't find
- **Interpretable & documented** - you can't use what you can't comprehend
- **Trusted & secure** - you can't use what's been tampered with, lost, or destroyed
- **Traceable to process** - data stemming from a process should bear some mark (metadata) of the particulars of the process that generated it
	- Ideally a specific, serialized activation of the process; but at a minimum a [[Process Specification]] of some kind.
- **Consistent & standardized** - the fewer anomalies and differences you have within a given dataset or between similar types of datasets, the easier they are to work with
	- Example: dates should use [[ISO 8601]], unless the database technology has built-in [[Data Types|Date Types]].
- **Complete** - sort of a facet of being "Trustable", but you shouldn't unknowingly have missing data

---
### Source
- 

### Related
- 