---
aliases: [homogeneous]
--- 

#recursion-induction 

## Definition 

> [!tldr] Definition
> A recurrence relation is **homogeneous** if the relation is given only in terms of prior terms, with no references to other quantities except for constant multiples of prior terms. 

Notes: 
- A homogeneous [[Linear recurrence relation|linear]] recurrence relation can be solved using the [[characteristic root method]]. 

## Examples and Non-Examples

* Example: $a_0 = 1$, $a_1 = 2$; and for $n > 1$, $a_n = 2a_{n-1} + 5a_{n-2}$. This is a second-[[Recurrence relation|order]] homogeneous recurrence relation because the relation to prior terms, found on the right side, consists only of (constant multiples of) prior terms. 
* * Example: $a_0 = 1$, $a_1 = 2$; and for $n > 1$, $a_n = 2a_{n-1} + 5a_{n-2} + 5n$. This is a *non-homogensous* recurrence relation because of the added term of $5n$, which is not a prior term in the sequence.  
* Example: $a_0 = 4$; and for $n > 0$, $a_n = 3a_{n-1}$ is a first-[[Recurrence relation|order]] homogeneous recurrence relation because the relation to prior terms, found on the right side, consists only of (constant multiples of) a prior term. 
* Example: $a_0 = 4$; and for $n > 0$, $a_n = 3a_{n-1} + 10$ is non-homogeneous because of the added $10$; this is not a prior term of the sequence and that's why this is nonhomogeneous. 

## Resources 

![](https://www.youtube.com/watch?v=4c6Bg2GJvQw)