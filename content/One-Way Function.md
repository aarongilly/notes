---
aliases: trapdoor function
tags: [math, coding]
---
**Easy to do one way, difficult to do the other**

One way functions are vital for [[Public Key Encryption]]. The example given from the source involves [[Modular Arithmetic]] and [[Primitive Root]]s:

![[IMG_9434.jpeg]]

Another example they gave was mixing together two colors of paint. It's easy to mix them to get the 3rd color in the middle, but would be exceedingly difficult to undo.

A subset of 'one-way functions' a *trapdoor function* is a one-way function **that becomes easy given a piece of information**.

A great example from the Wikipedia source:
> An example of a simple mathematical trapdoor is:
> "6895601 is the product of two prime numbers. What are those numbers?" 
> A brute-force solution would be to try dividing 6895601 by many prime numbers until finding the answer. However, if one is told that 1931 is one of the numbers, one can find the answer by entering "6895601 ÷ 1931" into any calculator.

---
### Source
- [Kahn Academy]([](https://www.khanacademy.org/computing/computer-science/cryptography/modern-crypt/v/diffie-hellman-key-exchange-part-1))

### Related
- [[Primitive Root]]
- [[Modular Arithmetic]]
- [[Prime Numbers]]
- [[Public Key Encryption]]
 