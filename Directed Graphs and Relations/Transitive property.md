---
aliases:
  - transitive
  - transitive relation
tags:
  - digraphs-relations
created: 2024-10-24
updated:
---
---
## Definition 

> [!tldr] Definition
> A [[Relation|relation]] $R$ on a set $X$ is said to be **transitive** if, for any $a,b,c \in X$, if $(a,b) \in R$ and $(b,c) \in R$, then $(a,c) \in R$. 

**Notes**: 
* A relation *fails* to be transitive if there are pairs $(a,b)$ and $(b,c)$ in $R$, but $(a,c) \not \in R$. 
* If we view the relation $R$ as a [[Directed graph|directed graph]], then the relation is transitive if it is already equal to its [[Transitive closure|transitive closure]]. 

## Examples

* Let $\sim$ be the "rhymes with" relation on the set of all English words, so $w \sim v$ if word $w$ rhymes with word $v$. If word $u$ rhymes with word $v$ (example: "book" rhymes with "nook")  and word $w$ rhymes with word $v$ ("nook" rhymes with "look") then $u$ rhymes with $w$ ("book" rhymes with "look"). So this relation is transitive. 
* Define a relation $\sim$ on the set $X = \{1,2,3,4,5,6\}$ using the following rule: $a \sim b$ [[Biconditional statement|if and only if]] $a$ [[Divisibility|divides]] $b$ (that is, $b$ is a multiple of $a$). Suppose $a \sim b$ and $b \sim c$. This means that $a$ divides $b$ and $b$ divides $c$, or alternatively that $b$ is a multiple of $a$ and $c$ is a multiple of $b$. So write $b = k_1a$ and $c =k_2b$. Then substituting, we get $c = k_2(k_1a)$ which is $c = (k_2k_1)a$. Therefore $c$ is a multiple of $a$ and so $a \sim c$. Therefore this relation is transitive.  
* Define a relation $\sim$ on the set $\mathbb{Z}$ of all [[Integers|integers]] by declaring $a \sim b$ if $|b-a| \leq 3$. So for example, $10 \sim 12$ because $|12 - 10| \leq 3$. This relation is *not* transitive: We saw that $10 \sim 12$, and similarly $12 \sim 14$ because $|14-10| \leq 3$. But $10 \not \sim 14$ because $|14 - 10| > 3$.

## Resources 

![](https://www.youtube.com/watch?v=-IdDcwEGKbc)

