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

- The [[Euclidean Algorithm|Euclidean algorithm]] can be used to compute the GCD and is usually the mathematical foundation for GCD functions in programming languages. 
## Examples 

| $a$  | $b$  | $\gcd(a,b)$ |
| ---- | ---- | ----------- |
| 3    | 15   | 3           |
| 3    | 10   | 1           |
| 10   | 14   | 2           |
| 2025 | 2030 | 5           |
| -15  | 10   | 5           |
| 0    | 99   | 99          |
| 0    | 0    | undefined   |

- Row 4 shows that negative [[integers]] can be involved in GCD computations; however the GCD is always positive, by definition. 
- Row 5 shows that one of the two [[integers]] can be zero; if so, then the GCD is automatically the absolute value of the second [[Integers|integer]] since every [[Integers|integer]] [[Divisibility|divides]] zero. 
- Row 6 reiterates the point that we cannot compute a GCD with both [[integers]] being zero. 

## Resources 

![](https://www.youtube.com/watch?v=jFd-6EPfnec)
