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
* Define a relation $\sim$ on the set $\mathbb{Z}$ of all [[Integers|integers]] by declaring $a \sim b$ if $|b-a| \leq 3$. So for example, $10 \sim 12$ because $|12 - 10| \leq 3$. This relation is *not* transitive: We saw that $10 \sim 12$, and similarly $12 \sim 14$ because $|14-10| \leq 3$. But $10 \not \sim 14$ 


## Resources 

(video)

Other resources: 
- 

## Practice 
