---
tags:
  - math
  - modeling
  - art music
created: 2023-07-08T11:37-05:00
updated: 2023-07-09T10:44-05:00
---
**Raster = Pixel Maps, Vector = Content Described by Code**

There are two main approaches to storing images on a computer: using bitmaps (**Raster Images, aka Bitmaps**) and using mathematical formulas to describe them (**Vector Images)**. 

## Bitmaps (Raster)

A pure bitmap (not compressed into any sort of compression format, like "jpeg" or "gif") would describe a grid of pixels, each of which with a certain number of bits reserved to describe their color content (typically an even number of bytes, 8 bit, 16 bit, and so on). A pure bitmap could say that the top-left pixel is pure red. So, pixel in position 0,0 has an RGB value of (255, 0, 0). 

## Vectors

Vector images are stored as lines of code. This is fundamentally different from the bitmap approach. A simple "[[SVG]]" file, when opened in a text-editor, can be pretty easily parsed by a human with some graph paper. Since mathematical formulas can describe continuous curves, you can infinitely zoom in or out on a Vector image and not lose fidelity. 

---

## Source
- [Vector art: What is vector art? | Adobe](https://www.adobe.com/creativecloud/illustration/discover/vector-art.html)

### Related Notes
- [[SVG]]