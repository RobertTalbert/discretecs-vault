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
> **Kuratowski's Theorem** states that a finite [[Graph|graph]] is [[Planar graph|planar]] if and only if it does not contain a [[Subgraph|subgraph]] that is a [[subdivision]] of $K_5$ (the [[Complete graph|complete graph]] on 5 vertices) or $K_{3,3}$ the [[Bipartite graph|complete bipartite graph]] with 3 vertices in each partition. 

## Examples 

Kuratowski's Theorem implies that $K_n$ is nonplanar for every $n \geq 5$, since such a graph either is $K_5$ itself or contains a subgraph isomorphic to $K_5$. 

The theorem would also conclude that this graph is nonplanar: 
![[Pasted image 20240724103305.png]]
This is because there is a copy of $K_{3,3}$ contained in it: One partition is $\{l,b,e\}$ and the other is $\{a,c,g\}$. ([Source](https://math.stackexchange.com/questions/2476097/is-this-graph-a-planar-graph-or-not))

## Resources

- [A proof of Kuratowski's Theorem](https://www.math.cmu.edu/~mradclif/teaching/228F16/Kuratowski.pdf)