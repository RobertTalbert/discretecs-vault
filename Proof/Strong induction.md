---
aliases:
  - strong induction
tags:
  - proof
  - recursion-induction
created: 2024-07-09
updated:
---
---
## Definition 

> [!tldr] Definition
> **Strong induction** is a proof technique, a variation on [[Mathematical induction|mathematical induction]] which is used to prove that a [[Predicate|predicate]] $P(n)$ is true for all natural numbers or a [[subset]] of the natural numbers. Like regular mathematical induction, strong induction proofs follow a three-step framework: 
> 
> 1. (*Base case*) Establish, by direct computation or demonstration, that $P(n)$ is true for the smallest value of $n$ for which it is claimed to be true. That is, establish that the base case leads to a true statement.  
> 2. (*Inductive hypothesis*) Assume that the predicate $P(n)$ is true for **all natural numbers less than or equal to a specified natural number $k$.**
> 3. (*Inductive step*) Prove that $P(k+1)$ is true, using a combination of the inductive hypothesis, the recursion involved in the predicate, previously-proven results, and so on. 
>    
>The bold-face part of step 2 is the difference between strong induction and [[Mathematical induction|mathematical induction]]. See Notes below. 

**Notes**:
- Regular [[Mathematical induction|mathematical induction]] is sometimes referred to as *weak induction* to distinguish it from strong induction. 
- The difference between strong and weak induction is in the second step of the framework. Whereas weak induction only assumes that the predicate is true for a single, unspecified natural number $k$, strong induction assumes that the predicate is true for $k$ **and for all other natural numbers less than $k$.**  
- Strong induction is a good choice of proof technique if there is no clear logical way to deduce that $P(k+1)$ is true simply from knowing that $P(k)$ is true, but there is a logical way to deduce $P(k+1)$ is true if the predicate is true for some smaller input value. See examples below. 
- Strong and weak induction are [[Logical equivalence|logically equivalent]] in the sense that if one of these methods is logically valid, so is the other. ([Proof of the equivalence](https://mathcenter.oxford.emory.edu/site/math125/strongInductionEquivalence/))

## Examples 

> [!NOTE] **Claim**: Given $n \in \mathbb{N}$, define $a_n$ [[Recursion|recursively]] as follows: $a_0 = 1$, $a_1 = 3$, and $a_n = 2a_{n-1} - a_{n-2}$ for all $n > 1$. Then $a_n = 2n+1$ for all $n \geq 0$. 
> 
> **Proof**: We use strong induction. The base case is $n=0$. We are given that $a_0 = 1$, and if we plug in $n=0$ to $2n+1$ we get $1$ as well. So the base case holds. 
> 
> Now assume that for some natural number $k$, every natural number $i \leq k$ satisfies $a_i = 2i+1$. We want to show that $a_{k+1} = 2(k+1) + 1$. 
> 
> By the recursive definition, $a_{k+1} = 2a_k - a_{k-1}$. Now the inductive hypothesis applies to both terms on the right: 
> $$a_k = 2k+1 \qquad a_{k-1} = 2(k-1)+ 1$$
> So we can substitute: 
> $$a_{k+1} = 2(2k+1) - (2(k-1) + 1) = 4k + 2 - (2k-2+1) = 4k+2 - 2k + 1 = 2k+3 = 2(k+1) + 1$$
> This is what we wanted to prove. ◼



> [!note] **Claim:** Every positive integer $n \geq 2$  is either a [[Prime and composite numbers|prime number]] or is a product of prime numbers. 
> 
> **Proof**: We use strong induction. The base case is when $n=2$. In this case $n=2$ is known to be prime, so the base case holds. 
> 
> Now assume that for some natural number $k$, every natural number less than or equal to $k$ is either prime, or a product of primes. We want to prove that $k+1$ is either prime or a product of primes. Clearly either $k+1$ is prime or it is composite (there are no other options). If $k+1$ is prime, then we are done. So assume that that $k+1$ is composite; we want to show that $k+1$ is a product of primes. Since $k+1$ is composite, factor it into $k+1 = ab$ with $a,b > 1$. Since $a$ and $b$ are both factors of $k+1$, they are smaller than $k+1$. Hence they are less than or equal to $k$, so the inductive hypothesis says that each one is either a prime number or a product of prime numbers. Let's assume that $a = p_1p_2\cdots p_s$ and $b = q_1q_2\cdots q_t$ where each $p$ and each $q$ is a prime number. (If $a$ or $b$ is itself a prime number, there would be only one number in the list of factors.) Then since $k+1 = ab$, we can write 
> $$k+1 = (p_1p_2\cdots p_s)(q_1q_2 \cdots q_t)$$
> which establishes that $k+1$ is a product of prime numbers. This is what we set out to prove. ◾
> 

## Resources 

![](https://www.youtube.com/watch?v=n-bJB_7QbQU)