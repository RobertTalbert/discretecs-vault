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
- A proof of Ore's Theorem is found in the video below. 
- 

## Example

In the graph below, $n = 6$ (the number of vertices). 
![[ore-example.png]]
The degree of each vertex is either 3 or 5, and every vertex other than vertex 1 is adjacent to vertex 1. So if $u$ and $v$ are non-adjacent, it must be that $\deg(u)$ and $\deg(v)$ both equal 3, so $\deg(u) + \deg(v) = 6$ which is greater than or equal to 6. Ore's Theorem would then guarantee that $G$ has a Hamilton circuit. By examining the graph, we can see that this is indeed the case, for example $1, 2, 4, 3, 6, 5, 1$ is a Hamilton circuit. 

Another example: Consider the [[Bipartite graph|complete bipartite graph]] $K_{4,4}$:  
![[k44.png]]

There are $n=8$ vertices in this graph, and any two nonadjacent vertices must come from the same partition, and have degree 4. Therefore $\deg(u) + \deg(v) = 8$ for all nonadjacent vertices $u$ and $v$. Since this is greater than or equal to $n=8$, $K_{4,4}$ has a Hamilton circuit. An example of a such a circuit can be built by picking a vertex and alternating back and forth between the partitions and choosing different vertices each time, and ending at the starting vertex. 

## Resources 

![](https://www.youtube.com/watch?v=r0IHSXkSSGE)
