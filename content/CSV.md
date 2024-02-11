---
created: 2023-07-08
aliases: 
tags:
  - data
---
**The plaintext relational data storage format.**

CSV stands for "Comma Separated Value" or "Common Separated Variable". It's the simplest possible data dump for structured data (arguably aside from [[JSON]]). The structure, though, is very limited to simple, flat tables. CSV does not lend itself to modeling hierarchical data (like JSON or [[XML]]) or object-oriented data.

CSV files can have different "flavors", but each of which has at least these two things:

1. The delimiter - traditionally a comma
2. The new line indicator - traditionally a carriage return/"new line" character
3. Often there will also be a way to "escape" these characters to allow for their use *in* the data. A common method is the use of a "text qualifier".

There are a few different standards for CSV.

- Internet W3C tabular standard
- RFC 4180 standard

### Example

```
This is a single element,
"this, too, is a single element",
"This element, named ""bob"", is also one element"
```

## Issues

CSV files contain **only** data. There is no standard universal method of wrapping up metadata into a CSV file. This means there is no way to explicitly "[[Data Types|type]]" a given field. There may or may not be headers naming the columns.

Parsing issues are common between CSV programs that use slightly different flavors.

The data are not always *that* human-readable.

---

### Source

### Related
- [[JSON]] 
- [[Relational Databases]] 
- [[Plain Text Durability]] 
- [[Data Serialization]] 
- [[Data Serialization Methods]]