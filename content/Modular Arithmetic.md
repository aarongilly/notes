---
created: 2023-07-23
aliases: 
tags: [math, coding]
---
**A system of arithmetic that considers the *remainder* of division**.

Modular arithmetic is nothing more than "math that uses the modulus operator". As a reminder, the modulus operator is just short for the algorithm: 

`A mod B` is the same as "Take A, divide by B, give me the remainder."

In [[JavaScript]] it's expressed using the percent sign:

```javascript
let a = 16 % 10
console.log(a) //logs `6`
```

Modular arithmetic shows up in [[Public Key Encryption]], and when you're doing anything that involves iterating through a set, and starting back at the beginning. A common place would be adding a set number of hours to a time of day.
$$10pm + 30 hours = 4am$$
You go around the 24 hour clock once, then have 6 hours left over, which takes you to 11, 12, 1, 2, 3, and end up at 4.

It shows up in analysis of the game "Set", per the source video below.

For some reason you use the term ''[[Congruent]]" when doing modulus operations?
	13 mod 4 "is congruent to" 1...
		Perhaps because when applied to the 'going around a circle' way of thinking, they form the same angle?

****
### Source
- school
- Kahn Academy Public Key Encryption tutorial
- this video:
- ![Video](https://www.youtube.com/watch?v=EkFX9jUJPKk&t=698s)

### Related
- [[Public Key Encryption]]
 