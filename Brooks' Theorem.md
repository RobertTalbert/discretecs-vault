---
aliases: 
tags:
  - graphs
created: 2024-07-24
updated:
---
---
## Definition 

> [!tldr] Definition
> **Brooks' Theorem** states that any graph $G$ satisfies the inequality $\chi(G) \leq \Delta(G)$ where $\chi(G)$ is the graph's [[Chromatic number|chromatic number]] and $\Delta(G)$ is its [[Degree|maximum degree]], unless $G$ is a [[Complete graph|complete graph]] or an odd [[Paths|cycle]], in which case $\chi(G) = \Delta(G) + 1$. 

Notes: 
- Brooks' Theorem is useful as a way to place an upper bound on the [[Chromatic number|chromatic number]] of a graph, or in the case of a [[Complete graph|complete graph]] or odd [[Paths|cycle]] to compute the chromatic number outright. 
- Brooks' Theorem is similar to but different than [[Vizing's Theorem]] which is a [[Theorem|theorem]] about [[Edge coloring|edge coloring]]. 

## Examples 

Consider this graph $G$ with 10 vertices and 15 edges: 
![[random-graph-723.png|500]]
By visual inspection, $\Delta(G) = 6$. Brooks' Theorem would say that $\chi(G) \leq 6$ since this graph is clearly not a [[Complete graph|complete graph]] or an odd cycle. Also note that the chromatic number must be *at least* 3, since there are copies of $K_3$ (a triangle) in the graph and at least three different colors are needed . Therefore we know from this information alone that $3 \leq \chi(G) \leq 6$. In fact the actual [[Chromatic number|chromatic number]] is exactly 3, as seen directly from this coloring: 


## Resources 

(video)

Other resources: 
- 

## Practice 
