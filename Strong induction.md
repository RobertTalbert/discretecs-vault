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




## Resources 

(video)

Other resources: 
- 

## Practice 
