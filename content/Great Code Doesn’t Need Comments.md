---
aliases: 
tags:
  - coding
---
**If you need comments to explain your code, it's not great code.**

Great code it's readable by itself. Comments aren't necessary, and in fact can be a bad thing. They are a crutch for explaining bad code… AND they have to be maintained separately from the code. Comments will lie to you, when details or requirements change and the code is updated, but the comments aren’t.

## Example

Comment-dependent by bad code

```jsx
//only update if the data date is over one month old or the user is an admin
if(record.date < new Date().setMonth(new Date().getMonth() - 1) || user.priviledge >= 3){
  flagForUpdate(records);
}

```

Same functionality without comments

```jsx
const LAST_MONTH = new Date().setMonth(new Date().getMonth() - 1);
const OUT_OF_DATE = record.date < LAST_MONTH;
const USER_IS_ADMIN = user.privilege >= 3;

if(OUT_OF_DATE || USER_IS_ADMIN){
  flagForUpdate(record);
} 
```

---

### Source
[https://youtu.be/Bf7vDBBOBUA](https://youtu.be/Bf7vDBBOBUA)

### Related
- [[Don't Nest Your Code]]
- [[Code Auto-Documentation]]