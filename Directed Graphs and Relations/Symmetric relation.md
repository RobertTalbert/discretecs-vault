---
aliases:
  - symmetric
  - symmetric relation
tags:
  - digraphs-relations
created: 2024-10-24
updated:
---
---
## Definition 

> [!tldr] Definition
> A [[Relation|relation]] $R$ on a set $X$ is said to be **symmetric** if, for any $a,b \in X$, if $(a,b) \in R$ then $(b,a) \in R$. 

Notes: 
- A relation *fails* to be symmetric if there is a pair $(a,b) \in R$ such that $(b,a) \not \in R$. 
- If we view the relation $R$ as a [[Directed graph|directed graph]], the relation is symmetric if every directed edge has a directed edge pointing in the opposite direction. 

## Examples and Non-Examples

* Let $\sim$ be the "rhymes with" relation on the set of all English words, so $w \sim v$ if word $w$ rhymes with word $v$. If word $w$ rhymes with word $v$ (example: "book" rhymes with "nook") then $v$ also rhymes with $w$ ("nook" rhymes with "book") so this relation is symmetric. 
* Define a relation $\sim$ on the set $\mathbb{Z}$ of all [[Integers|integers]] by declaring $a \sim b$ if $|b-a| \leq 3$. So for example, $10 \sim 12$ because $|12 - 10| \leq 3$. Now if $a \sim b$ this means $|b -a| \leq 3$. If this is the case then $|a-b| \leq 3$ as well, because $|b-a| = |a-b|$. Therefore if $a \sim b$, it is also true that $b \sim a$. So this relation is symmetric. 
* Define a relation $\sim$ on the set $X = \{1,2,3,4,5,6\}$ using the following rule: $a \sim b$ [[Biconditional statement|if and only if]] $a$ [[Divisibility|divides]] $b$ (that is, $b$ is a multiple of $a$). This relation is *not* symmetric: For example $2 \sim 6$ because $2$ divides $6$, but $6$ does not divide $2$ so $6 \not \sim 2$. 

## Resources 
![](https://www.youtube.com/watch?v=URvVflKoBgw)

