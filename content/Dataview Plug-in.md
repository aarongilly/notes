---
created: 2023-08-04
aliases: 
tags: [notetaking]
---
summary::**A very powerful [[Obsidian]] plug-in**.

Dataview makes Obsidian *way* more useful.

## Dataview Uses
#### Finding Orphaned Pages
```dataview 
list 
from "" where length(file.inlinks) =0 and length(file.outlinks) = 0 
```
#### Based On A Property
```dataview
TABLE created
WHERE created
SORT created DESC
LIMIT 70
```

#### Finding Pages Edited Recently
```dataview
TABLE dateformat(file.mtime, "yyyy-MM-dd HH:mm") AS "Last modified"
FROM ""
SORT file.mtime DESC
LIMIT 5
```

#### Finding & Displaying Notes with Certain Fields
```dataview
TABLE summary
WHERE summary 
```

---
### Source
- 

### Related
- [[Obsidian]]
- [[Obsidian Niceties]]
 