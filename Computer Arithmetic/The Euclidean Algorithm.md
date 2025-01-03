---
aliases:
  - Euclidean algorithm
tags:
  - computer-arithmetic
created: 2025-01-03
updated:
---
---
## Definition 

> [!tldr] Definition
> The **Euclidean Algorithm** is a process that uses the [[The division algorithm|Division Algorithm]] repeatedly to find the [[Greatest common divisor|greatest common divisor]] of two [[Integers|integers]]. 
> 
> The algorithm generally runs as follows: We start with two integers $a$ and $b$, at least one of which is nonzero. 
> 
> - If $a = 0$, then return $\gcd(a,b) = b$ as the result and stop, because $\gcd(0,b) = b$ as long as $b$ is nonzero. 
> - If $b = 0$, then return $\gcd(a,b) = a$ as the result and stop, because $\gcd(a,0) = a$ as long as $b$ is nonzero. 
> - Otherwise: 
> 	- Use the [[The division algorithm|Division Algorithm]] to write $a = bq + r$ (i.e. divide $a$ by $b$ to get a quotient, $q$ and remainder, $r$).
> 	- Reassign the variables by setting $a = b$ and then $b = r$. 
> 	- Now com


(blurb)

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 
