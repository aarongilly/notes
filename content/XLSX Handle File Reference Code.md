---
tags:
- coding
---
**Snippet inside.**

```tsx
let inputElement = document.querySelector('#myInput')!;
inputElement.addEventListener('change',handleFile,false);
    return comp;
}

async function handleFile(event:Event) {
    const input = event.target as HTMLInputElement;
    if (!input.files?.length) {
        throw new Error('No file passed into the handleFile call');
    }
    const file = input.files[0];
    const ext = file.name.split(".")[file.name.split(".").length - 1];
    if(ext === 'json'){
        console.log('json dropped');
        const json = await file.text();
        const obj = JSON.parse(json);
        console.log(obj);
        
    }else if(ext === 'xlsx' || ext === 'csv' || ext === 'xlsm'){
        console.log('Excel dropped');
        const data = await file.arrayBuffer();
        let wkbk = XLSX.read(data);
        console.log(wkbk);
    
    }else{
        throw new Error('Unsupported file type: .' + ext)
    }    
}
```

---

## Source


### Related Notes