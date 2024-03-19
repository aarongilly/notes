---
created: 2023-07-08
aliases: 
tags:
  - clarity
  - modeling
  - coding
---
**Unified Syntax Tree - a generic structured data building block standard**

“Unist” is short for “Unified Syntax Tree” - it is intended to function as an Abstract Base Class for more purpose-built extensions. It is a basic, [[JSON]]-based, hierarchical organizational scheme.

At it’s core, it’s a tree built around nodes:

```tsx
interface Node {
  type: string
  data: Data?
  position: Position?
}
```

Nodes may contain other nodes. If so, they extend the Parent interface:

```tsx
interface Parent <: Node {
  children: [Node]
}
```

The purpose of the Unist is to provide a common basic hierarchical structure to create utilities that can be then reused between different applications of Unist. Examples would be utilities for tree traversal, path-finding, find, filter, et cetera.

Although the word [[Ontology]] doesn’t appear anywhere in the GitHub, Unist feels **very similar** to the concept of an [[Ontology]] Representation Language. 

Some [[Markdown Processers]] (like Remark) are capable of putting out HTML ************and/or************ Unist-structured JSON. [[Markdown]] in Unist is called “Mdast”. 

The API for [[Notion]] reveals their data structure is either Unist-compliant or is heavily inspired by Unist.

## Example Markdown Implementation (from Remark)

### Input

```markdown
> Alpha bravo charlie.
```

### Output

```json
{
  type: 'blockquote',
  children: [{
    type: 'paragraph',
    children: [{type: 'text', value: 'Alpha bravo charlie.'}]
  }]
}
```

****
### Source
[https://github.com/syntax-tree/unist](https://github.com/syntax-tree/unist)

### Related
- [[Markdown]] 
- [[Notion]] 
- [[Ontology]]