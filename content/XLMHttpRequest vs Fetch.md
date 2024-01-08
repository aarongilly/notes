---
aliases: 
tags:
  - coding
---
**Requesting http stuff.**

### Source
- [[freeCodeCamp]]

```jsx
const req = new XMLHttpRequest();
req.open("GET",'/json/cats.json',true);
req.send();
req.onload = function(){
  const json = JSON.parse(req.responseText);
  document.getElementsByClassName('message')[0].innerHTML = JSON.stringify(json);
};
```

equivalent:

```jsx
fetch('/json/cats.json')
    .then(response => response.json())
    .then(data => {
        document.getElementById('message').innerHTML = JSON.stringify(data);
    })
```

### Related
- [[Code References]]