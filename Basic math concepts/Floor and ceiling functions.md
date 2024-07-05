---
aliases:
  - floor function
  - ceiling function
  - Floor function
  - Ceiling function
tags:
  - basic-concepts
created: 2024-07-01
updated:
---
---
## Definition 

> [!tldr] Definition
> 1. The **floor function**, denoted $f(x) = \lfloor x \rfloor$, is a [[Function|function]] from the set of real numbers to the set of [[Integers|integers]] defined by taking the input and rounding down to the next lower integer. 
> 2. The **ceiling function**, denoted $g(x) = \lceil x \rceil$, is a [[Function|function]] from the set of real numbers to the set of [[Integers|integers]] defined by taking the input and rounding up to the next higher integer. 

Notes: 
- In Python, the floor and ceiling functions are accessed by first loading the `math` library and then accessing `floor` or `ceil` as methods: 

```python
import math
math.floor(3.4)
# Result: 3

import math # Not necessary to load this a second time 
math.ceil(3.4)
# Result: 4
```

* In *Mathematica*, the floor and ceiling functions are `Floor` and `Ceiling`. ([Floor documentation](https://reference.wolfram.com/language/ref/Floor.html); [Ceiling documentation](https://reference.wolfram.com/language/ref/Ceiling.html))
```mathematica
Floor[-4.5]
> -5

Ceiling[-4.5]
> -4
```
## Examples 

|  Expression to evaluate   | Result                                   |
| :-----------------------: | ---------------------------------------- |
|   $\lfloor 3.4 \rfloor$   | $3$                                      |
|    $\lceil 3.4 \rceil$    | $4$                                      |
| $\lfloor 3.99999\rfloor$  | $3$                                      |
| $\lceil 3.0000001 \rceil$ | $4$                                      |
|    $\lfloor 5 \rfloor$    | $5$                                      |
|  $\lfloor -4.3 \rfloor$   | $-5$ (go down to the next lower integer) |
|   $\lceil -5.6 \rceil$    | $-5$ (go up to the next higher integer)  |

## Resources 

![](https://youtu.be/wIbM2nece9s?si=gU5nbc5njdmFX30T)

