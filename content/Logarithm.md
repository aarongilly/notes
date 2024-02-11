---
created: 2023-07-08
aliases: 
tags:
  - math
---
**The inverse of Exponents.**

> [!tldr] 💁 $\log_z(x)=y$  →  $z^y=x$

## Logarithm Properties

All of these properties hold for any base number.

### Log of Multiplication

Multiplication within a Log turns into addition of two logs.

$$
\log_a(x\times y) = \log_a(x) + \log_a(y)
$$

### Log of Division

Division within a Log turns into subtraction of two logs.

$$
\log_a(\frac{x}{y}) = \log_a(x) - \log_a(y)
$$

### Log of Exponentiation

Exponents within a Log can be moved outside the log as coefficients.

$$
\log_a(x^y)=y\times \log_a(x)
$$

### Change-of-Base

You can do this, for any number "b":

$$
\log_a(x) = \frac{\log_b(x)}{\log_b(a)}
$$

So, if you want $\log_3(x)$ and your calculator only has buttons for "LOG" and "LN", you can just use: $\frac{\ln(x)}{\ln(3)}$.

$$
\log_8(15) = \frac{\log_2(15)}{\log_2(8)} \approx 1.3023
$$

## Special Logarithms

- Log Base 10: "The Common Logarithm"
    
    $\log(x)=y$    →    $10^y=x$
    
    "Common" because it was commonly used before calculators as a way to turn division into subtraction. With a slide rule & a table of the answers to $\log(x)$ you could figure out $\log_x(y)$ for any x or y.
    
- Log Base *e*: "The Natural Logarithm"
    
    $\ln(x)=y$    →    $e^y=x$
    
    The Natural Logarithm is related to continuously compounding growth. 
    
    If you have an investment with 5% annually compounding interest, how long will it take to double? 
    
    $\ln(2)=0.693={rate}\times{time}$
    
    $0.693 = 0.05 \times {time}$
    
    $\frac{0.693}{0.05} = {time} = 13.86$ years
    
- Log Base 2a: "The Binary Logarithm"
    
    $log_2(x)=y$    →    $2^y=x$
    
    Useful in knowing the number of digits necessary to representing a given number in binary, or how many layers a head-to-head bracket will require.

---

### Source

### Related
- [[Logarithms & Exponents]]