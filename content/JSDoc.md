---
created: 2023-07-08
aliases: 
tags:
  - coding
---
**The correct syntax for writing comments in [[JavaScript]]**

If you want your tools to work *with* you, use JSDoc. It is what [[Intellisense]] draws from. It enables [[TypeScript]]-like type checking regardless of whether or not you’re actually *using* TypeScript. 

Example from my [[PDW]] :

```tsx
/**
 * Singleton pattern.
 * @returns the PDW
 */
public static getInstance(): PDW {
    if (!PDW.instance) {
        PDW.instance = new PDW();
    }
    return PDW.instance;
}
```

---

### Source

### Sources

[Jsdoc cheatsheet](https://devhints.io/jsdoc)

[Use JSDoc: Index](https://jsdoc.app/)

### Related
- [[TypeScript]] 
- [[Intellisense]]