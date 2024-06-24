---
aliases:
  - proof by contrapositive
tags:
  - proof
  - logic
created: 2024-06-24
updated: 2024-06-24
---
---
## Definition 

> [!tldr] Definition
> A **proof by contrapositive** is a [[Proof|proof]] of a [[Conditional statements|conditional statement]] in which a [[Direct proof|direct proof]] is given for the [[Contrapositive|contrapositive]] of that statement. 

Notes: 
- Since the [[Contrapositive|contrapositive]] of a conditional statement is [[Logical equivalence|logically equivalent]] to the original conditional statement, any correct proof of one suffices as a proof for the other. 
- The contrapositive of a conditional statement is sometimes easier to prove than the original statement, particularly if the original statement involves [[Negation|negations]]. See examples below. 
- A proof by contrapositive is simply a [[Direct proof|direct proof]] of a different statement, so the structure of such a proof is the same as any direct proof: First assume the (new) hypothesis, then proceed using definitions, computations, previously-proven results, or basic facts to explain why the (new) [conclusion](app://obsidian.md/Conditional%20statements) is true.

## Examples 

> [!NOTE] Proof involving even and odd integers
>  
> **Prove: For any integer $n$, if $n^2$ is even, then $n$ is even.**
> 
> Note: This would be a difficult statement to prove with a [[Direct proof|direct proof]]. We would first assume that $n^2$ is even, then we would need to prove that $n$ is even. But there is no obvious way to start with information about $n^2$ and conclude information about $n$, other than taking a square root, which introduces a complicated operation into the picture. It's much simpler to prove the contrapositive. 
> 
> **Proof:** We will prove the contrapositive instead, which states: *If $n$ is odd, then $n^2$ is odd.* So assume that $n$ is [[Even and odd integers|odd]], which means $n = 2k+1$ for some integer $k$. We want to show that $n^2$ is also odd, that is, $n^2 = 2q + 1$ for some integer $q$. Use basic algebra to compute $n^2$: 
> $$n^2 = (2k+1)^2 = 4k^2 + 4k + 1 = 2(2k^2 + 2k) + 1$$ Since $k$ is an integer, so is $2k^2 + 2k$ by [[Closure of the integers|closure]]. This shows that there is an integer $q$, namely $q = 2k^2 + 2k$, such that $n^2 = 2q+1$. Therefore $n^2$ is odd. ◼


**Prove: For any real number $x$, if $x^3 - x > 0$ then $x > -1$. 

Note: Again, a [[Direct proof|direct proof]] presents some tactical difficulties here. We would have to assume that $x^3 - x > 0$ and then prove somehow that $x > -1$. This would involve relatively complex algebra reasoning, perhaps by factoring $x^3 - x$ into $x(x-1)(x+1)$ and then explaining why 

## Resources 

(video)

Other resources: 
- 

## Practice 
