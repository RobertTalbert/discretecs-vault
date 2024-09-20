---
aliases: 
tags:
  - graphs
created: 2024-09-20
updated:
---
---
## Definition 

> [!tldr] Definition
> **Ore's Theorem** states that: 
> If $G$ is a [[Graph|graph]] with $n$ [[Graph|vertices]] with $n \geq 3$, such that $\deg(u) + \deg(v) \geq n$ for every pair of nonadjacent vertices $u$ and $v$, then $G$ has a [[Hamiltonian path and circuit|Hamilton circuit]]. 

Notes: 
- Ore's Theorem is one of a small number of results that give conditions which, when met, guarantee the existence of a [[Hamiltonian path and circuit|Hamilton circuit]]. However, it is not "constructive" -- it does not say how to find or build the circuit. 
- The [[Converse|converse]] of Ore's Theorem is not true. That is, if $G$ has a [[Hamiltonian path and circuit|Hamilton circuit]] we cannot  conclude anything about the degrees of the vertices in $G$. A simple example where the converse is not satisfied is $C_5$, the [[Cycle graph|cycle graph]] on 5 vertices (which looks like a pentagon). Clearly $C_5$ has a Hamilton circuit (pick one vertex and go around the entire graph). In this graph, $n=5$. But the degree of each vertex in $C_5$ is 2, so $\deg(u) + \deg(v) = 4$ for every pair of nonadjacent vertices, which is strictly less than $5$. 

## Example






## Resources 

(video)

Other resources: 
- 
