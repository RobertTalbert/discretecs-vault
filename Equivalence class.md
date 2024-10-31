---
aliases:
  - equivalence class
tags:
  - digraphs-relations
created: 2024-10-31
updated:
---
---
## Definition 

> [!tldr] Definition
> Suppose $\sim$ is an [[Equivalence relation|equivalence relation]] on a set $X$, and $a \in X$. Then the **equivalence class** of $a$, denoted $[a]$,  is the set of all elements of $X$ that are related to $a$. That is: 
> $$[a] = \{ x \in X \, : \, a \sim x \}$$

Notes: 
- Since an [[Equivalence relation|equivalence relation]] is [[Symmetric property|symmetric]], we can replace $a \sim x$ in the definition with $x \sim a$. 
- The equivalence class of an element $a$ is always nonempty, since $a \in [a]$ due to equivalence relations being [[Reflexive property|reflexive]]. 
- Two equivalence classes must be either [[Intersection|disjoint]] or equal. That is, given $a,b \in X$, either $[a] \cap [b] = \emptyset$ or $[a] = [b]$. 
- Given an [[Equivalence relation|equivalence relation]] on $X$, the collection of equivalence classes forms a partition of $X$, that is, the equivalence classes are mutually [[Intersection|disjoint]] and their [[Union|union]] makes up the entire set $X$. Conversely, any partition of a set defines an [[Equivalence relation|equivalence relation]] by declaring $x \sim y$ if $x$ and $y$ belong to the same set in the partition. 

## Examples 

- Let $\sim$ be the relation on the set $\{0, 1, 2, \dots, 99\}$, such that $a \sim b$ if $a \, \% \, 10 = b \, \% \, 10$ where $\%$ is the [[The modulus operator|modulus operator]]. Then $[14] = \{4, 14, 24, 34, 44, 54, 64, 74, 84, 94\}$. And, $[0] = \{0, 10, 20, 30, 40, 50, 60, 70, 80, 90\}$. 
- Let $\sim$ be the relation on the set of all US cities with populations over 1,000,000 people such that $c_1 \sim c_2$ if $c_1$ and $c_2$ are in the same US state. 

## Resources 

(video)

Other resources: 
- 

## Practice 
