---
aliases: 
tags:
  - coding
  - data
---
**Scalable Vector Graphics - a text-based representation of images.**

Scalable Vector Graphics are images that are drawn by computers according to human-readable [[XML]]-based instructions. They are stored with the file extensions `.svg`. They are opposed to bitmap-type (or "Raster") images, which describe a literal map of what color pixels go in which places. Instead they describe how lines and shapes are drawn, how thick they are, what color they are, what their transparency is, etc. This allows you to infinitely zoom in on a SVG and never see pixelization.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Scalable_Vector_Graphics)

### Example

Open the content of a ".svg" file in notepad you see:

```xml
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<svg width="391" height="391" viewBox="-70.5 -70.5 391 391" xmlns="http://www.w3.org/2000/svg">
<rect fill="#fff" stroke="#000" x="-70" y="-70" width="390" height="390"/>
<g opacity="0.8">
<rect x="25" y="25" width="200" height="200" fill="lime" stroke-width="4" stroke="pink" />
	<circle cx="125" cy="125" r="75" fill="orange" />
	<polyline points="50,150 50,200 200,200 200,100" stroke="red" stroke-width="4" fill="none" />
	<line x1="50" y1="50" x2="200" y2="200" stroke="blue" stroke-width="4" />
</g>
</svg>
```

Open it in a browser or image viewer and you see (minus the grid):

![Example](SVG_example.svg)

Source: [Wikipedia](https://en.wikipedia.org/wiki/Scalable_Vector_Graphics)

---

### Source
- [[Coding]]
- [[Data]]
- [[XML]]
- [[Wikipedia](https://en.wikipedia.org/wiki/Scalable_Vector_Graphics)](Untitled%2027.png)

Source: ]]

### Related
- [[XML]] 
- [[Data Serialization]]