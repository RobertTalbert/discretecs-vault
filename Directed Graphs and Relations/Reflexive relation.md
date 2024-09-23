---
aliases:
  - reflexive
  - reflexive relation
tags:
  - digraphs-relations
created: 2024-09-23
updated:
---
---
## Definition 

> [!tldr] Definition
> A [[Relation|relation]] $R$ on a set $X$ is said to be **reflexive** if $(a,a) \in R$ for all $a \in X$. 

Notes: 
- In other words a relation is reflexive if every element of the ground set $X$ is related to itself. 

## Examples and Non-Examples

* Define a relation $\sim$ on the set $X = \{1,2,3,4,5,6\}$ using the following rule: $a \sim b$ [[Biconditional statement|if and only if]] $a$ [[Divisibility|divides]] $b$ (that is, $b$ is a multiple of $a$). Then, since every element of $X$ divides itself (according to the definition of [[Divisibility|divides]]) this is a reflexive relation. 
* Define another relation, also called $\sim$, on the set $X = \{1,2,3,4,5,6\}$ by declaring $a \sim b$ [[Biconditional statement|if and only if]] $b \, \% \, a = 2$ (where `%` is the [[The modulus operator|modulus operator]]). Then, since $2 \, \% \, 2 \neq 2$, we see that $2$ is not "related to" itself and therefore this is not a reflexive relation. As a set, this relation is $\{(3, 2), (4, 2), (5, 2), (6, 2), (3, 5), (4, 6) \}$, and by direct inspection we can see that $(2,2)$ does not belong to it. 
* Viewed as a [[Directed graph|directed graph]], a relation would be reflexive if every node in the graph had an edge pointing to itself, i.e. every node has a self-loop. 

## Resources 

(video)

Other resources: 
- 

## Practice 
