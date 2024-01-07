---
tags:
  - notetaking
summary: URLs to open to spots within your vault from OUTSIDE Obsidian.
created: 2023-07-08T20:47-05:00
updated: 2024-01-06T23:10-06:00
---
**`= this.summary`**

You can create [[URI]]s to **navigate** to specific notes, headings, and even blocks within [[Obsidian]]. They can also be used to **create notes** and do other things too!

## URL to Open
To note:
`obsidian://open?vault=Notes&file=Obsidian%20URIs`

To Heading:
`obsidian://open?vault=Notes&file=Obsidian%20URIs%23URL%20to%20Open`

To block:
`obsidian://open?vault=Notes&file=Obsidian%20URIs%23%5Eabcde`

> [!hint] Blocks must be given IDs like so. ^abcde

## URL to Search
`obsidian://search?vault=Notes&query=Obsidian`

## URL to Create
`obsidian://new?vault=Notes&name=my%20new%20note`

Supports:
- `content`
- `append`
- `overwrite`
- `silent` - creates without opening

---
### Source
- [Obsidian Docs](https://help.obsidian.md/Concepts/Obsidian+URI)

### Related
- [[Obsidian vs Notion]]