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

## Examples and Non-Examples

Let $\sim$ be the "rhymes with" relation on the set of all English words, so $w \sim v$ if word $w$ rhymes with word $v$. This relation is [[Reflexive property|reflexive]] (every word rhymes with itself), [[Symmetric property|symmetric]] (if word 1 rhymes with word 2, then word 2 rhymes with word 1) and [[Transitive property|transitive]] (if word 1 rhymes with word 2 and word 2 rhymes with word 3 then word 1 rhymes with word 3). So it is an equivalence relation. 

## Resources 

(video)

Other resources: 
- 

## Practice 
