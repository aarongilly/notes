---
created: 2023-07-08
aliases: 
tags:
  - coding
---
**Any function whose output is ONLY dependent on its input.**

In coding, [[Functions]] may be pure or impure. Impure functions produce outputs that depend on **not only** their inputs, but also rely on some ambient variable or some sort of 3rd party “state”.

## Examples

```jsx
//#Impure
let carColor = "blue";
function carDesc(){ 
  return `Wow! a ${carColor} car!`
}

//#Pure
function carDesc(color){ 
  return `Wow! a ${color} car!`
}
```

 Often, impure functions are class methods dependent on the state of some class instance properties.

****
### Source

### Related
- [[Functions]]