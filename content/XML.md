---
tags:
- coding
- modeling
- data
---
**Extensible Markup Language - a document encoding markup language.**

XML (*Extensible Markup Language*) is a very widely-used well-supported markup language, upon which many many many document formats have been constructed. Office documents are typically XML-based. As are [[SVG]]s, RSS feeds, and hundreds of other types. XML is a form of [[Data Serialization]] and is hierarchical (tree-based).

## Components

All characters in an XML document are either *markup* characters or *content* characters. Markup strings are surrounded by `<` and `>` or `&` and `;`. Everything else is content.

### Tags

Tags are what's contained within the less than and greater than symbols. Tags contain a text-based identifier that informs how elements should be parsed. For example `<img>` identifies an the element represents an image.

### Elements

Elements are a a chunk of xml contained between matching opening and closing tags.

### Attributes

Attributes are name-value pairs inserted into the tag next to the tag identifier to supply supplemental data, such as the `src` attribute in an image tag: `<img src="whatever.jpg">`

### XML Declaration

XML documents begin with a declaration that describe how they are formatted (what standard they are using, what character encoding, etc).

## Example

```xml
<greeting>Hello there, <lie>friend</lie>.</greeting>
```

---

## Source

[XML - Wikipedia](https://en.wikipedia.org/wiki/XML)

### Related Notes
- [[JSON]] 
- [[YAML]] 
- [[Data Serialization]]