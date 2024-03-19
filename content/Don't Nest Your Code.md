---
created: 2023-07-08
aliases: 
tags:
  - coding
---
**If your code is more than 3 levels deep, then you should probably re-factor.**

Nested code is much harder to read much harder to reuse and much harder to maintain. Also, where you are at in the hierarchy of nests changes the context of what variables are available and what the situation is. If your code is more than three levels deep, you should probably refactor. Extract out functions. Move error conditions to the top rather than using “ELSE” statements. 

Be a ‘Never Nester’.

# Example from My Code

### Before

```tsx
constructor(inputData: MinimumElement) {
		//...
		if(inputData._deleted !== undefined){
        if(typeof inputData._deleted === 'boolean'){
            this._deleted = inputData._deleted;
        }else if(typeof inputData._deleted === 'string'){
            this._deleted = (<string>inputData._deleted).toUpperCase() === 'TRUE';
        }else if(typeof inputData._deleted === 'number'){
            this._deleted = (<number>inputData._deleted) === 1 ? true : false;
        } else {
            console.warn(`Didn't know how to set '_deleted' based on input. Defaulting to 'false':`, inputData._deleted);
            this._deleted = false 
        }
    }else{
			this._deleted = false
		}
		//...
}
```

### After

```tsx
constructor(inputData: MinimumElement){
	//...
	this._deleted = handleDeletedInputVariability(inputData._deleted);
	//...
}

// extraction & "never nesting" really made this code way more readable... huh
private handleDeletedInputVariability(deletedVal: any): boolean{
    if (deletedVal === undefined) return false
    if (typeof deletedVal === 'boolean') return deletedVal;
    if (typeof deletedVal === 'string') return (<string>deletedVal).toUpperCase() === 'TRUE';
    if (typeof deletedVal === 'number') return (<number>deletedVal) === 1 ? true : false
    console.warn(`Didn't know how to set '_deleted' based on input. Defaulting to 'false':`, deletedVal);
    return false 
}
```

****
### Source

### Source

[Why You Shouldn't Nest Your Code](https://youtu.be/CFRhGnuXG-4)

### Related
- [[~7 - The Limit of Simultaneous Info]] 
- [[Simplicity]]