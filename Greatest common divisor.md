---
aliases:
  - GCD
  - gcd
  - greatest common divisor
tags:
  - computer-arithmetic
created: 2025-01-03
updated:
---
---
## Definition 

> [!tldr] Definition
> The **greatest common divisor** or **GCD** of two [[Integers|integers]], which are not both zero, is the largest positive [[Integers|integer]] that [[Divisibility|divides]] both of them. 

**Notes**: 
- The greatest common divisor of $a$ and $b$ is denoted $\gcd(a,b)$. 
- The GCD is sometimes called the *greatest common factor* or GCF. 
- In Python, the GCD is available as a function in the `math` module. Here is an example of use: 

```python
from math import gcd
gcd(10,14)

> 2
```

- The [[The Euclidean Algorithm|Euclidean algorithm]] can be used to compute the GCD and is usually the mathematical foundation for GCD functions in programming languages. 
## Examples 

| $a$ | $b$ | $\gcd(a,b)$ |
| --- | --- | ----------- |
| 3   | 15  | 3           |
| 3   | 10  | 1           |
| 2   |     |             |
 

## Resources 

(video)

Other resources: 
- 

## Practice 
