---
created: 2023-08-04T18:47-05:00
updated: 2023-09-21T15:56-05:00
---
[summary::**A very powerful [[Obsidian]] plug-in**.]


Dataview makes Obsidian *way* more useful.

## Dataview Uses
#### Finding Orphaned Pages
```dataview 
list 
from "" where length(file.inlinks) =0 and length(file.outlinks) = 0 
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

#### Tags
#notetaking 