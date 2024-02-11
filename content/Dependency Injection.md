---
created: 2023-08-04
aliases: 
tags: [coding, technique]
---
**Passing code into the function that depends on it.**

Hard to describe. Easy to understand through example. 

## Benefits:
- separation of concerns
	- thereby all the benefits of that, modularity, etc

## Example
### Dependent Code
```typescript
//not using dependency injection
class Entry{
  private data: any;
  private saveSpot: "local" | "cloud"
  //these arguments are optional sometimes, required others
  //logic for how to interact with the save location is buried
  //inside the Entry object
  save(directory?: string, cloudCredentials?: string){
    if(this.saveSpot === "local"){
      //code to save locally 
      //depends on directory arg
      return
    }
    if(this.saveSpot === "cloud"){
      //code to save to cloud
      //depends on cloud arg
      return
    }
  }
} 
```

### With Dependency Injection
```typescript
interface iSaveSpot{
  save(): function
}

class localSave implements iSaveSpot{
  private directory: string
  constructor(loc: string){
    this.directory = loc;
  }
  save(){
    //code to save locally here
  }
}

class cloudSave implements iSaveSpot{
  private credentials: object
  constructor(creds: object){
	  this.credentials = creds;
  }
  save(){
    //code to save to cloud here
  }
}

class Entry{
  private data: any;
  private saveSpot: saveSpotInterface
  save(){
	//zero dependent code, Entry doesn't have to know
	//where it's saving or what specific things have
	//to happen to perform the save function
    this.saveSpot.save();
  }
} 

```

---
### Source
- ![Code Aesthetic](https://youtu.be/J1f5b4vcxCQ)

### Related
- [[Code Design Patterns]]
 