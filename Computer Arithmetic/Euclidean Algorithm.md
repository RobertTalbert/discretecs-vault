---
aliases:
  - Euclidean algorithm
  - the Euclidean Algorithm
tags:
  - computer-arithmetic
created: 2025-01-03
updated: 2025-01-06
---
---
## Definition 

> [!tldr] Definition
> The **Euclidean Algorithm** is a process that uses the [[Division algorithm|Division Algorithm]] repeatedly to find the [[Greatest common divisor|greatest common divisor]] of two [[Integers|integers]]. 
> 
> The algorithm generally runs as follows: We start with two [[integers]] $a$ and $b$, at least one of which is nonzero. 
> 
> - If $a = 0$, then return $\gcd(a,b) = b$ as the result and stop, because $\gcd(0,b) = b$ as long as $b$ is nonzero. 
> - If $b = 0$, then return $\gcd(a,b) = a$ as the result and stop, because $\gcd(a,0) = a$ as long as $b$ is nonzero. 
> - Otherwise: 
> 	- Use the [[Division algorithm|Division Algorithm]] to write $a = bq + r$ (i.e. divide $a$ by $b$ to get a quotient, $q$ and remainder, $r$).
> 	- Reassign the variables by setting $a = b$ and then $b = r$. 
> 	- Find $\gcd(a,b)$ using the Euclidean Algorithm ([[Recursion|recursively]]) with the new values of $a$ and $b$. 
> 	  
> Eventually the remainder $r$ will become zero, at which point one of the first two steps will activate and the algorithm will stop. 


**Notes**: 
- The Euclidean Algorithm is [[Recursion|recursive]]: It computes a number by running itself on smaller inputs. 
- In Python, the Euclidean Algorithm can be implemented non-[[Recursion|recursively]] as follows, using the [[Modulus operator|modulus operator]] `%` to get the remainder when dividing `a` by `b`:
```python
def euclidean_algorithm(a,b):
	while b != 0:
		a,b = b, a % b
	return abs(a)
```

## Examples 

Let's use the Euclidean Algorithm to find $\gcd(500,336)$. Here we will set $a = 500$ and $b = 336$. 

1. Neither $a$ nor $b$ is zero, so we go to the third bullet in the algorithm use the [[Division algorithm|Division Algorithm]] to divide $a$ by $b$. Doing so gives us $500 = (336)(1) + 164$. The remainder is $r = 164$. 
2. Reassign the variables to set $a = 336$ and $b = 164$. Neither is zero, so the algorithm doesn't stop yet. 
3. Use [[Division algorithm|the Division Algorithm]] on the new values: $336 = (164)(2) + 8$. That is, the remainder is $r = 8$. 
4. Reassign variables to set $a = 164$ and $b = 8$. These are not zero, so we continue. 
5. Divide again to get $164 = (8)(20) + 4$. That is, the remainder is $r = 4$. 
6. Reassign variables to set $a = 8$ and $b = 4$. These are not zero, so continue. 
7. Divide again to get $8 = (4)(2) + 0$. This time the remainder is $0$. 
8. Reassign variables to set $a = 4$ and $b=0$. Since one of these is zero, the algorithm stops, and returns the absolute value of the other one: $\gcd(500,336) = 4$. 

Summarized in a table, this looks like:

| Step | $a$ | $b$ | Remainder when dividing $a$ by $b$ |
| ---- | --- | --- | ---------------------------------- |
| 1    | 500 | 336 | 164                                |
| 2    | 336 | 164 | 8                                  |
| 3    | 164 | 8   | 4                                  |
| 4    | 8   | 4   | 0                                  |
| 5    | 4   | 0   | 4 ◀ This is the [[Greatest common divisor\|GCD]]                |
 
## Resources 

![](https://www.youtube.com/watch?v=JUzYl1TYMcU)

Although he misspelled "Euclidean" 😢

**Other resources:** 
- [Calculator that uses the Euclidean Algorithm and shows the steps](https://www.calculatorsoup.com/calculators/math/gcf-euclids-algorithm.php) 

