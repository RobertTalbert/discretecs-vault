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
> **Dirac's Theorem** states: 
> If $G$ is a [[Graph|graph]] with $n \geq 3$ vertices, and the degree of each vertex is at least $n/2$, then $G$ has a [[Hamiltonian path and circuit|Hamilton circuit]]. 

Notes: 
- Dirac's Theorem is a corollary to [[Ore's Theorem]]: If the conditions of Dirac's Theorem are met, that is $\deg(u) \geq n/2$ for all vertices $u$, then let $x$ and $y$ be non-[[Adjacent|adjacent]] vertices; we know that $\deg(x) \geq n/2$ and $\deg(y) \geq n/2$ because this was assumed to be true for all vertices. Then, $\deg(x) + \deg(y) \geq n/2 + n/2 = n$, so [[Ore's Theorem]] implies the existence of a [[Hamiltonian path and circuit|Hamilton circuit]]. 
- The converse of Dirac's Theorem is not true: It is possible for a graph $G$ to have a Hamilton circuit, but not all vertices have degree greater than or equal to 2. A simple counterexample is $C_5$, the [[Cycle graph|cycle graph]] on $5$ vertices, which has a Hamilton cycle but the degree of each vertex is less than $5/2$. 
- Two different proofs of Dirac's Theorem (one of which repeats the first bullet above) are given in the video below. 

## Examples 

Consider this graph with $n=8$ vertices: 
![[dirac-example.png]]
The degree sequence of the graph is 6, 6, 5, 5, 5, 5, 4, 4. We can see from here that the degree of each vertex is greater than or equal to $8/2 = 4$. Dirac's Theorem would then imply that $G$ has a [[Hamiltonian path and circuit|Hamilton circuit]]. Dirac's Theorem gives only the *existence* of this circuit; it doesn't say what it is, or how to find it. However, working with the graph some more would uncover 1, 4, 7, 3, 6, 5, 2, 8, 1 as an example [[Hamiltonian path and circuit|Hamilton circuit]]. 


## Resources 

![](https://www.youtube.com/watch?v=S7bORlkfwsA)