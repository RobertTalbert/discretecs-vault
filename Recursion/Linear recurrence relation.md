---
aliases: [linear]
--- 

#recursion-induction 

## Definition 

> [!tldr] Definition
> A recurrence relation is **linear** if the prior terms used in the recurrence relation are combined only through addition of constant multiples of those terms. 

Notes: 
- A [[Homogeneous recurrence relation|homogeneous]] linear recurrence relation can be solved using the [[characteristic root method]]. 

## Examples and Non-Examples

* Example: $a_0 = 1$, $a_1 = 2$; and for $n > 1$, $a_n = 2a_{n-1} + 5a_{n-2}$. This is a second-[[Recurrence relation|order]] linear recurrence relation because the only thing being done to the prior terms on the right side of the recurrence relation is addition of constant multiples of the terms. 
* Example: $a_0 = 4$; and for $n > 0$, $a_n = 3a_{n-1}$ is a first-[[Recurrence relation|order]] linear recurrence relation because the only thing being done to the one prior term on the right side, is multiplication by a constant. 
* Example: $a_0 = 1$, $a_1 = 4$, $a_2 = 5$; and for $n >2$, $a_n = 3a_{n-1} - 2a_{n-2} + 6a_{n-3}$ is a third-[[Recurrence relation|order]] linear recurrence relation. 
* **Non-example:** $a_0 = 4$; and for $n > 0$, $a_n = \sqrt{a_{n-1}}$  is a *non-linear* linear recurrence relation because we are not just multiplying by a constant, we are taking a square root of the prior term. 
* **Non-example**: $a_0 = 1$, $a_1 = 2$; and for $n > 1$, $a_n = a_{n-1} \cdot a_{n-2}$. This is a nonlinear recurrence relation because we are not simply adding constant multiples of the prior terms together, we are multiplying the prior terms themselves.


## Resources 

![](https://www.youtube.com/watch?v=4c6Bg2GJvQw)

