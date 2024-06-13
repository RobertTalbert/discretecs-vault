---
aliases:
  - divides
  - divisibility
tags:
  - basic-concepts
created: 2024-06-13
updated:
---
---
## Definition 

> [!tldr] Definition
> If $a$ and $b$ are two [[integers]], then we say **$b$ divides $a$** and write $b | a$ if there exists an integer $k$ such that $a = bk$. 

Notes: 
- If $b$ divides $a$, we can also say that $a$ is a multiple of $b$. 
- Note that the notation $a|b$ is not the fraction $a/b$ or $b/a$. The vertical bar is not a fraction bar, but shorthand for a statement about the relationship between $a$ and $b$. 
- Divisibility is a special case of the [[The division algorithm|Division Algorithm]] in which there is no remainder. That is, if $a$ and $b$ are integers, the Division Algorithm states that there must be integers $q$ and $r$ with $0 \leq r < b$ such that $a = bq + r$. If $r = 0$ in this case, then $b | a$. 
- If an integer $b$ *does not* divide the integer $a$, then we indicate this by putting a slash through the vertical bar: $b \nmid a$.  

## Examples and Non-Examples

* $10 | 200$ because $200 = 20(10)$. 
* However $10 \nmid 25$ because when dividing $25$ by $10$ we get a nonzero remainder. 
* We can apply the definition of divisibility to situations where long division doesn't readily apply, for example with negative numbers: We see that $-12 | -48$ because $-48 = 4(-12)$. 
* The number $0$ is divisible by every other integer. Let $a$ be any integer whatsoever. Then $0 = 0\cdot a$, which by definition says that $a | 0$. (This is true even if $a = 0$ itself!)
* However, $0$ does not divide any integer except $0$ itself. If $b$ were an integer and $0 | b$, then there would have to be another integer $q$ such that $b = q \cdot 0$. But if $b$ is nonzero, this is impossible because the right side of that equation always equals $0$. (This is an example of an [[indirect proof]].)

## Resources 

![](https://www.youtube.com/watch?v=K2YmMpulFA4)