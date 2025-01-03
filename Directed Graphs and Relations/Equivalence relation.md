---
aliases:
  - equivalence relation
tags:
  - digraphs-relations
created: 2024-10-31
updated:
---
---
## Definition 

> [!tldr] Definition
> An **equivalence relation** is a [[relation]] that is [[Reflexive property|reflexive]], [[Symmetric property|symmetric]], and [[Transitive property|transitive]]. 

Notes: 
- The three properties required for an equivalence relation are the essential properties of mathematical relations that are similar to "equality". 

## Examples and Non-Examples

- Let $\sim$ be the "rhymes with" relation on the set of all English words, so $w \sim v$ if word $w$ rhymes with word $v$. This relation is [[Reflexive property|reflexive]] (every word rhymes with itself), [[Symmetric property|symmetric]] (if word 1 rhymes with word 2, then word 2 rhymes with word 1) and [[Transitive property|transitive]] (if word 1 rhymes with word 2 and word 2 rhymes with word 3 then word 1 rhymes with word 3). So it is an equivalence relation. 
- Let $\sim$ be the relation on the set $\mathbb{Z}$ of all integers, such that $a \sim b$ if $a \, \% \, 10 = b \, \% \, 10$ where $\%$ is the [[Modulus operator|modulus operator]]. This is an equivalence relation. 
- Let $\sim$ be the relation on the set $\mathbb{Z}$ of all integers, such that $a \sim b$ if $a < b$. While this relation is [[Transitive property|transitive]], it is **not** an equivalence relation because it is not [[Reflexive property|reflexive]]: For example $1 \not < 1$. 
- Let $\sim$ be the relation on the set $\mathbb{Z}$ of all integers, such that $a \sim b$ if $a \leq b$. While this relation is [[Reflexive property|reflexive]] and [[Transitive property|transitive]], it is **not** an equivalence relation because it is not [[Symmetric property|symmetric]]: For example $1 \leq 2$ but $2 \not \leq 1$. 
- Let $\sim$ be the relation on the set $\mathbb{Z}$ of all integers, such that $a \sim b$ if $|a - b| \leq 5$. While this relation is [[Reflexive property|reflexive]] and [[Symmetric property|symmetric]], it is **not** an equivalence relation because it is not [[Transitive property|transitive]]: For example $1 \sim 4$ since $|1-4| \leq 5$ and $4 \sim 7$ since $|4-7| \leq 5$, but $1 \not \sim 7$ because $|1-7| > 5$. 

## Resources 

![](https://www.youtube.com/watch?v=T6RUxvJR8i4)_

