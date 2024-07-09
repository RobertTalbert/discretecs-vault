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
> **Strong induction** is a proof technique, a variation on [[Mathematical induction|mathematical induction]] which is used to prove that a [[Predicate|predicate]] $P(n)$is true for all natural numbers or a [[subset]] of the natural numbers. Like regular mathematical induction, strong induction proofs follow a three-step framework: 
> 
> 1. (*Base case*) Establish, by direct computation or demonstration, that $P(n)$ is true for the smallest value of $n$ for which it is claimed to be true. That is, establish that the base case leads to a true statement.  
> 2. (*Inductive hypothesis*) Assume that the predicate $P(n)$ is true for **all natural numbers less than or equal to a specified natural number $k$.**
> 3. (*Inductive step*) Prove that $P(k+1)$ is true, using a combination of the inductive hypothesis, the recursion involved in the predicate, previously-proven results, and so on. 
>    
>    The bold-face part of step 2 
> 
> 
> a [[proof]] technique used when proving that a [[Predicate|predicate]] $P(n)$ (whose [[Domain|domain]] is the set of all [[Natural numbers|natural numbers]]) is true for all natural numbers or for some specified [[Subset|subset]]. It is especially applicable if the predicate involves [[Recursion|recursion]]. Induction proofs follow a three-step **framework**: 
> 1. (*Base case*) Establish, by direct computation or demonstration, that $P(n)$ is true for the smallest value of $n$ for which it is claimed to be true. That is, establish that the base case leads to a true statement.  
> 2. (*Inductive hypothesis*) Assume that $P(k)$ is true for some random, undisclosed value of $k$. 
> 3. (*Inductive step*) Prove that $P(k+1)$ is true, using a combination of the inductive hypothesis, the recursion involved in the predicate, previously-proven results, and so on. 

(blurb)

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 
