---
tags:
  - digraphs-relations
created: 2024-10-24
updated: 
aliases:
  - antisymmetric
  - antisymmetric relation
  - antisymmetry
---

---
## Definition 

> [!tldr] Definition
> A [[Relation|relation]] $R$ on a set $X$ is said to be **antisymmetric** if, for any $a,b \in X$, if $(a,b) \in R$ and $(b,a) \in R$, then $a=b$. 

**Notes**: 
* In other words a relation is antisymmetric if there is no pair of _distinct_ elements of $X$ in a two-directional relationship with each other. 
* Viewed as a [[Directed graph|directed graph]], a relation would be antisymmetric if there are no pairs of directed edges that point in both directions between two nodes. 
* A relation would *fail* to be antisymmetric if 

## Examples

* Define a relation $\sim$ on the set $X = \{1,2,3,4,5,6\}$ using the following rule: $a \sim b$ [[Biconditional statement|if and only if]] $a$ [[Divisibility|divides]] $b$ (that is, $b$ is a multiple of $a$). Suppose $a \sim b$ and $b \sim c$. This means that $a$ divides $b$ and $b$ divides $c$, or alternatively that $b$ is a multiple of $a$ and $c$ is a multiple of $b$. So write $b = k_1a$ and $c =k_2b$. Then substituting, we get $c = k_2(k_1a)$ which is $c = (k_2k_1)a$. Therefore $c$ is a multiple of $a$ and so $a \sim c$. Therefore this relation is transitive.  
* Define a relation $\sim$ on the set $\mathbb{Z}$ of all [[Integers|integers]] by declaring $a \sim b$ if $|b-a| \leq 3$. So for example, $10 \sim 12$ because $|12 - 10| \leq 3$. This relation is *not* transitive: We saw that $10 \sim 12$, and similarly $12 \sim 14$ because $|14-10| \leq 3$. But $10 \not \sim 14$ because $|14 - 10| > 3$.
* Let $\sim$ be the "rhymes with" relation on the set of all English words, so $w \sim v$ if word $w$ rhymes with word $v$. If word $u$ rhymes with word $v$ (example: "book" rhymes with "nook")  and word $w$ rhymes with word $v$ ("nook" rhymes with "look") then $u$ rhymes with $w$ ("book" rhymes with "look"). So this relation is transitive. 
* 

## Resources 

![](https://www.youtube.com/watch?v=-IdDcwEGKbc)

