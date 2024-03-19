---
created: 2024-02-26
tags:
  - notetaking
aliases:
  - JSON Canvas
---
[[Obsidian]] put out their own barebones [[Whiteboarding App]]-like feature called "Canvas" a while back. In March 2024 they rebranded to "[JSON Canvas](https://jsoncanvas.org/)". 

Canvas files are stored using a custom-build (but [[Open Source]]) file format "`.canvas`". It's simple [[JSON]], with a [[Graph Database]]-like structure. It's a map of `nodes` and `edges`.
### Example .`.canvas` File
```JSON
{
	"nodes":[
		{"id":"8edd2eb18bb22633","x":-725,"y":-460,"width":970,"height":1115,"color":"6","type":"group","label":"Embedding Scopes"},
		{"id":"6f4485d073444120","type":"text","text":"# Test.","x":-125,"y":100,"width":250,"height":60},
		{"id":"6ecb3caca2f6574f","x":-300,"y":-440,"width":400,"height":400,"type":"file","file":"Graphical Project Tracking.md"},
		{"id":"630672e28940268f","x":-160,"y":365,"width":385,"height":270,"type":"file","file":"Graphical Project Tracking.md","subpath":"#^fa9d7d"},
		{"id":"49cf666e52e28e24","type":"file","file":"Graphical Project Tracking.md","subpath":"#Tooling","x":-705,"y":230,"width":405,"height":200},
		{"id":"68099e202ff80fcf","type":"text","text":"# Buffalo","x":345,"y":-240,"width":250,"height":60},
		{"id":"774bb198ad025035","type":"file","file":"canvases/Exercise Canvas.canvas","x":395,"y":165,"width":400,"height":400},
		{"id":"1a7ec32d55357ee4","type":"text","text":"# Canvas Recursion","x":395,"y":-65,"width":400,"height":70},
		{"id":"282f505b11ff8cdc","type":"text","text":"### Search Target","x":470,"y":-440,"width":250,"height":60},
		{"id":"e33af1bf78938351","x":795,"y":-295,"width":484,"height":171,"type":"text","text":"# A More Substantial Card\nContains some stuff under the header. Including:\n- [x] A completed task!"}
	],
	"edges":[
		{"id":"9b8c442ebca200ed","fromNode":"1a7ec32d55357ee4","fromSide":"bottom","toNode":"774bb198ad025035","toSide":"top","label":"Works!"},
		{"id":"0d86052150747f56","fromNode":"282f505b11ff8cdc","fromSide":"bottom","toNode":"68099e202ff80fcf","toSide":"top","label":"Sadly doesn't work"},
		{"id":"9f19d3cd2e18fa5f","fromNode":"6f4485d073444120","fromSide":"top","toNode":"6ecb3caca2f6574f","toSide":"bottom","color":"3","label":"Embed to note"},
		{"id":"0b38f06899b34ca9","fromNode":"6f4485d073444120","fromSide":"left","toNode":"49cf666e52e28e24","toSide":"top","color":"4","label":"Embed to Heading"},
		{"id":"e0018e1d95a85f0a","fromNode":"6f4485d073444120","fromSide":"bottom","toNode":"630672e28940268f","toSide":"top","color":"5","label":"Embed to Block"}
	]
}
```

## Canvas Pros & Cons
### Pros 💪
- Like seemingly everything in Obsidian - canvas is **fast**.
- You can embed items into your canvas that look and work just like notes
- You can pull content from your vault easily
	- You can also "promote" parts of a canvas to full-blown standalone notes
- Support for link labels, groups, and coloring
- The file format makes a ton of sense and seems like I could expand on it
- Everything you can do on Canvas actually works really well from the iPad
### Cons 🫤
- Canvases are very much second-class citizens - and feel like it.
	- No support for backlinks
	- Search doesn't cover anything in Canvases
	- There's no [[Frontmatter]] or properties support
- There's no support for freehand drawings or anything
- "Groups" in the `.canvas` format don't actually have any sort of *explicit* membership, it looks like it's merely graphical overlap

****
### Source
- Playing wiht it
### Related
- [[Obsidian]]