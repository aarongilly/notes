---
aliases: 
tags: [math]
---
**Known as the 'Phi Function', tells how many numbers less than a number 'N' have no common factors (other than 1) with 'N'**

There's a formula for calculating this, but it was complicated. More important is what it is.

$$\phi(8) = 4$$
Phi of 8 equals 4 *because*:
8's factors are `[1, 2, 4, 8]`, and of the numbers less than 8:
- 1: factors: `[1]` ✅
- 2: factors `[1, 2]`  ❌ - shares `2`
- 3: factors `[1, 3]` ✅
- 4: factors `[1, 4]` ❌ - shares `4`
- 5: factors `[1, 5]` ✅
- 6: factors `[1, 2, 3, 6]` ❌ - shares `2`
- 7: factors `[1, 7]` ✅
And there are **4** numbers that share no common factors other than 1.

Another way of saying that is that there are 4 numbers less than 8 whose [[Greatest Common Factor|GCF]] is '1'.

Phi of any of the [[Prime Numbers]] is just that number - 1. Phi of 7 is 6. Phi of 11 is 10.

Weirdly, Phi is *multiplicative*, which means:
$$\phi(A*B)=\phi(A)*\phi(B)$$
THIS is (I think) what makes it useful in [[Public Key Encryption]]. 

---
### Source
- [Kahn Academy](https://www.khanacademy.org/computing/computer-science/cryptography/modern-crypt/v/euler-s-totient-function-phi-function)

### Related
- [[Public Key Encryption]]
- [[Primitive Root]]
 