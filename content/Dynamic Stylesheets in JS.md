---
created: 2023-07-08
aliases: 
tags:
  - coding
---
**You CAN affect the document’s stylesheets in JS... a couple of ways, actually.**

To manipulate global CSS (non-element CSS) using [[JavaScript]], you can create a `<style>` tag like any other HTML element. From there you’ve got a couple options for applying the styling.

1. Set innerHTML
    
    ```jsx
    var style = document.createElement('style');
    style.innerHTML = `
    #app {
    background-color: blueviolet;
    }
    `;
    document.head.appendChild(style);
    ```
    
2. Or use a method of [the CSSStyleSheet class](https://developer.mozilla.org/en-US/docs/Web/API/CSSStyleSheet).
    
    ```jsx
    var style = document.createElement('style');
    document.head.appendChild(style);
    style.sheet.insertRule('#app {background-color: darkseagreen}');
    
    //STYLESHEET MANIPULATION Option 2
    ```

---
### Source

[CSSStyleSheet - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/CSSStyleSheet)

[Set CSS styles with javascript](https://dev.to/karataev/set-css-styles-with-javascript-3nl5)

### Related
- [[Code References]]