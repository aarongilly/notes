---
created: 2023-08-04
aliases: 
tags: [notetaking]
---

summary::**A very powerful [[Obsidian]] plug-in**.

Dataview makes [[Obsidian]] *way* more useful.

## Dataview Uses
#### Note Count
This uses the [[JavaScript]] inline syntax.

> [!success] Currently there's **`$=dv.pages().length`** notes

#### Finding Orphaned Pages
```dataview 
list 
from "" where length(file.inlinks) =0 and length(file.outlinks) = 0 
```

#### Based On A Property
```dataview
TABLE created
WHERE created.year = 2024
SORT created DESC
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

#### Test
```dataview
TABLE
	length(rows.file.name) as notes
WHERE 
	file.tags 
FLATTEN 
	file.tags AS tag
WHERE 
	file.ctime.year = 2024
GROUP BY 
	tag 
SORT notes DESC
```
****
### Source
- 

### Related
- [[Obsidian]]
- [[Obsidian Niceties]]
 