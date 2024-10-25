---
tags:
  - digraphs-relations
created: 2024-10-24
updated: 2024-10-25
aliases:
  - antisymmetric
  - antisymmetric relation
  - antisymmetry
---

---
## Definition 

> [!tldr] Definition
> A [[Relation|relation]] $R$ on a set $X$ is said to be **antisymmetric** (or, "has the antisymmetric property") if, for any $a,b \in X$, if $(a,b) \in R$ and $(b,a) \in R$, then $a=b$. 

**Notes**: 
* In other words a relation is antisymmetric if there is no pair of _distinct_ elements of $X$ in a two-directional relationship with each other. 
* Viewed as a [[Directed graph|directed graph]], a relation would be antisymmetric if there are no pairs of directed edges that point in both directions between two nodes. 
* A relation would *fail* to be antisymmetric if there were at least one pair of distinct nodes, each of which was related to the other. 

## Examples

* Define a relation $\sim$ on the set $X = \{1,2,3,4,5,6\}$ using the following rule: $a \sim b$ [[Biconditional statement|if and only if]] $a$ [[Divisibility|divides]] $b$ (that is, $b$ is a multiple of $a$). Suppose $a \sim b$ and $b \sim a$. This means that $a$ divides $b$ and $b$ divides $a$, or alternatively that $b$ is a multiple of $a$ and $a$ is a multiple of $b$. So write $b = k_1a$ and $a =k_2b$. Then substituting, we get $a = k_2(k_1a)$ which is $a = (k_2k_1)a$. The only way this equation can hold is if $k_2k_1 = 1$, and since $k_2$ and $k_1$ are both integers, that would mean that either $k_1, k_2 = 1$ or $k_1, k_2 = -1$. The second option is impossible since $b = k_1a$ and $a,b$ are both positive. Therefore $k_1 = 1$ and so $b = a$ This proves that the divisibility relation is antisymmetric. 
* Define a relation $\sim$ on the set $\mathbb{Z}$ of all [[Integers|integers]] by declaring $a \sim b$ if $|b-a| \leq 3$. So for example, $10 \sim 12$ because $|12 - 10| \leq 3$. This relation is *not* antisymmetric: We saw that $10 \sim 12$, and similarly $12 \sim 10$ because $|12-10| \leq 3$. But clearly $10 \neq 12$.

## Resources 

![](https://www.youtube.com/watch?v=voqrhhVKj-A)

