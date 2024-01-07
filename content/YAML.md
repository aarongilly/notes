---
tags:
  - coding
  - data
created: 2023-07-08T11:37-05:00
updated: 2023-07-23T13:42-05:00
---
**Like JSON, but more human-readable.**

YAML is a space-dependent [[Data Serialization]] method, that extends upon JSON. It is highly flexible and has many features JDD AS IN lacks, but is more confusing to learn and also subject to type-inferencing errors if you're not paying attention.

A [[JSON]] string is also valid YAML, but a YAML string is probably not valid JSON. 

YAML is a way to provide metadata to a [[Markdown]] file & is used for coding configuration files. It can be used for general data storage. See also: [[YAML Uses]] 

There's a good [[NodeJS]] package that allows you to read/write to YAML using [[JavaScript]]. Can convert 1:1 to [[JSON]].

## Fast Facts

- Uses whitespace indentation (but not tabs)
- Can store multiple documents within a single file
- Comments start with #
- Lists can be done in two ways:
    1. [item 1, item 2] (like JSON)
    2. Or one per line, with the line starting with a hyphen
- Associative arrays (like Objects in JavaScript) can be done two ways:
    - {key: value} (like JSON)
    - with simple key, colon, space, value
- Strings typically aren't quoted, but can also be quoted or double-quoted
- Can have references and tags, using an Ampersand [[Sigil]] to denote the tag location and an asterisk sigil to reference it
    - The use of references allows for Graphs to be represented in YAML (not just trees, like JSON)

## Samples

```yaml
--- # The Smiths
- {name: John Smith, age: 33} #interoperability wiht JSON?
- name: Mary Smith
  age: 27
- [name, age]: [Rae Smith, 4]   # sequences as keys are supported
--- # People, by gender
men: [John Smith, Bill Jones]
women:
  - Mary Smith
  - Susan Williams
```

---

### Source
- [The Official YAML Web Site](https://yaml.org/)
- [What exactly is Frontmatter?](https://daily-dev-tips.com/posts/what-exactly-is-frontmatter/)
- [YAML - Wikipedia](https://en.wikipedia.org/wiki/YAML)

### Related Notes
- [[Data Serialization Methods]] 
- [[Data Serialization]] 
- [[YAML Uses]]