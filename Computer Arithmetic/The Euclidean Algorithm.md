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
> 	- Find $\gcd(a,b)$ using the Euclidean Algorithm ([[Recursion|recursively]]) with the new values of $a$ and $b$. 
> 	  
> Eventually the remainder $r$ will become zero, at which point one of the first two steps will activate and the algorithm will stop. 


**Notes**: 
- The Euclidean Algorithm is [[Recursion|recursive]]: It computes a number by running itself on smaller inputs. 
- In Python, the Euclidean Algorithm can be implemented non-recursively as follows, using the [[The modulus operator|modulus operator]] `%` to get the remainder when dividing `a` by `b`:
```python
def euclidean_algorithm(a,b):
	while b != 0:
		a,b = b, a % b
	return abs(a)
```

## Examples 

Let's use the Euclidean Algorithm to find $\gcd(500,2025)$. Here we will set $a = 2030$ and $b = 2025$. 

1. Neither $a$ nor $b$ is zero, so we go to the third bullet in the algorithm use the [[The division algorithm|Division Algorithm]] to divide $a$ by $b$. Acc



## Resources 

(video)

Other resources: 
- 

## Practice 
