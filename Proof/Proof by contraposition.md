---
aliases:
  - proof by contrapositive
  - proof by contraposition
tags:
  - proof
  - logic
created: 2024-06-24
updated: 2024-06-24
---
---
## Definition 

> [!tldr] Definition
> A **proof by contraposition** is a [[Proof|proof]] of a [[Conditional statements|conditional statement]] in which a [[Direct proof|direct proof]] is given for the [[Contrapositive|contrapositive]] of that statement. 

Notes: 
- Since the [[Contrapositive|contrapositive]] of a conditional statement is [[Logical equivalence|logically equivalent]] to the original conditional statement, a correct proof of one suffices as a proof for the other. 
- A proof by contrapositive is simply a [[Direct proof|direct proof]] of a different statement, so the structure of such a proof is the same as any direct proof: First assume the (new) hypothesis, then proceed using definitions, computations, previously-proven results, or basic facts to explain why the (new) [[Conditional statements|conclusion]] is true.
- The contrapositive of a conditional statement is sometimes easier to prove than the original statement, particularly if the original statement involves [[Negation|negations]], or if the contrapositive provides a [[Conditional statements|hypothesis]] whose assumption gives more useful information than the original hypothesis. See examples below. 

## Examples 

> [!NOTE] Proof involving even and odd integers
>  
> **Prove: For any integer $n$, if $n^2$ is even, then $n$ is even.**
> 
> Note: This would be a difficult statement to prove with a [[Direct proof|direct proof]]. We would first assume that $n^2$ is even, then we would need to prove that $n$ is even. But there is no obvious way to start with information about $n^2$ and conclude information about $n$, other than taking a square root, which introduces a complicated operation into the picture. It's much simpler to prove the contrapositive. 
> 
> **Proof:** We will prove the contrapositive instead, which states: *If $n$ is odd, then $n^2$ is odd.* So assume that $n$ is [[Even and odd integers|odd]], which means $n = 2k+1$ for some integer $k$. We want to show that $n^2$ is also odd, that is, $n^2 = 2q + 1$ for some integer $q$. Use basic algebra to compute $n^2$: 
> $$n^2 = (2k+1)^2 = 4k^2 + 4k + 1 = 2(2k^2 + 2k) + 1$$ Since $k$ is an integer, so is $2k^2 + 2k$ by [[Closure of the integers|closure]]. This shows that there is an integer $q$, namely $q = 2k^2 + 2k$, such that $n^2 = 2q+1$. Therefore $n^2$ is odd. ◼


> [!NOTE] Proof involving an inequality 
> 
> **Prove: For any real number $x$, if $x^3 - x > 0$ then $x > -1$.**
> 
> Note: Again, a [[Direct proof|direct proof]] presents some tactical difficulties here. We would have to assume that $x^3 - x > 0$ and then prove somehow that $x > -1$. This would involve relatively complex algebra reasoning, perhaps by factoring $x^3 - x$ into $x(x+1)(x-1)$ and then explaining why, if this expression is positive, that $x$ itself must be larger than $-1$. It seems simpler to start with simple information and work forward. 
> 
> An alternative proof of this statement using [[Indirect proof|indirect proof]] is shown in the article at the link. 
> 
> **Proof:** We will prove the contrapositive instead, which states: *If $x \leq -1$, then $x^3-x \leq 0$.* So, assume that $x \leq -1$. We want to show that $x^3 - x \leq 0$. Note that by factoring, we have $x^3 - x = x(x+1)(x-1)$. Given that $x \leq -1$, we know that the first and third terms  of this expression ($x$ and $x-1$) are both negative, so their product is positive. Therefore the sign of the entire expression is simply the sign of the middle term, $x+1$. If $x = -1$ then this is zero; if $x < -1$ then the sign of $x+1$ is negative. In either case the middle term, and therefore the entire expression, is less than or equal to zero. ◼

## Resources 

![](https://www.youtube.com/watch?v=hAFpc9abNFc)

![](https://www.youtube.com/watch?v=3ORYou8dc0s)
