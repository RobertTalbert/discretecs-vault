---
aliases:
  - Poset
  - poset
  - partially ordered set
  - partial ordering
  - Partial ordering
tags:
  - digraphs-relations
created: 2024-11-03
updated:
---
---
## Definition 

> [!tldr] Definition
> A **partial ordering** on a [[Set|set]] $X$ is a [[Relation|relation]] on $X$ that is [[Reflexive property|reflexive]], [[Antisymmetric property|antisymmetric]], and [[Transitive property|transitive]]. A set together with a partial ordering on the set is called a **partially ordered set** or *poset*. 

Notes: 
- A partial ordering mimics the "less than or equal to" relation on the set of [[Integers|integers]] (or any set of numbers). That relation, $\leq$, has the three properties given in the definition. 
- Because of this similarity with $\leq$, a partially ordered set can be [sorted](https://en.wikipedia.org/wiki/Sorting_algorithm). This makes posets of particular interest in computer science. 

## Examples and Non-Examples

- The "less than or equal to" relation ($\leq$) on $\mathbb{Z}$, the set of all integers, is a partial ordering. 
- On the set $\{1,2,3,\dots\}$ of positive integers, the "divides" relation (where $a \sim b$ if and only if $a$ [[Divisibility|divides]] $b$) is a partial ordering. 
- Given any set $W$ of words in a language, consider the relation where $w_1 \sim w_2$ if and only if $w_1$ comes before $w_2$ in alphabetical order. (For example $\text{car} \sim \text{cat}$ in the set of all English words). This relation is a partial ordering. 
- Let $X$ be any set and consider its [[Power set|power set]] ${\cal{P}}(X)$, with the relation that for all $A, B \subseteq X$ we say $A \sim B$ if and only if $A \subseteq B$. This is an equ 
- Given any set $W$ of words in a language, the relation where $w_1 \sim w_2$ if and only if $w_1$ rhymes with $w_2$ is *not* a partial ordering (although it is an [[Equivalence relation|equivalence relation]]) because the relation is not [[Antisymmetric property|antisymmetric]]: It's possible for $w_1$ to rhyme with $w_2$ and vice versa but $w_1 \neq w_2$ -- for example "cat" and "bat" rhyme with each other but are not the same word. 

## Resources 

(video)

Other resources: 
- 

## Practice 
