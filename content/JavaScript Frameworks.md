---
created: 2023-07-08
aliases: 
tags:
  - coding
---
**Some JavaScript tools & frameworks do all their lifting before the code is shipped.**

There are a **ton** of JavaScript frameworks. Most of them, like the big 3 most popular (React, Angular, and Vue) ship to the browser your code + supporting code they provide that you’re leveraging.

There is another breed of tools that do their work before the code is shipped, and produce clean, ideally very small packages for distribution to the browser. Svelte is a pure framework, just like React/Angular/Vue, but it does all of it’s work at *compile* time. What’s distributed to the browser is pure, clean JavaScript - with only the bits you’re actually using (thanks to [[Tree Shaking]]).

Not a *framework*, per say, but TypeScript is an entire *language* built around this concept. TypeScript is just JavaScript, with some added syntax to prevent errors, enhance tooling (enabling things like [[Code Auto-Documentation]]), and make it easier to scale JavaScript projects. What ultimately comes out the other side is just JavaScript.

---

### Source

### Related
- [[Tree Shaking]] 
- [[Code Auto-Documentation]]