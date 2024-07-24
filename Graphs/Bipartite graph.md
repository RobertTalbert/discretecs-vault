---
aliases:
  - bipartite
  - Bipartite
  - bipartite graph
  - complete bipartite graph
  - complete bipartite
  - Complete bipartite
tags:
  - graphs
created: 2024-07-24
updated:
---
---
## Definition 

> [!tldr] Definition
> A [[Graph|graph]] $G = (V,E)$ is **bipartite** if we can partition the [[Graph|vertex]] set $V$ into two nonempty, [[Intersection|disjoint]] [[Set|sets]], say $X$ and $Y$, such that every [[Graph|edge]] of the graph has exactly one [[Graph|endpoint]] in $X$ and one endpoint in $Y$. 
> 
> A bipartite graph in which each vertex in one of the partitions is [[Adjacent|adjacent]] to *every* vertex in the other partition, is called a **complete bipartite graph**. For a complete bipartite graph, if one of the partitions has $n$ vertices and the other has $m$, we denote it $K_{n,m}$. 


## Examples

The graph below is bipartite, with the partitions separated into red/numbers and blue/letters: 
![[bipartite1.png]]
It is bipartite because every edge has one endpoint in one of the partitions and the other endpoint in the other partition. However it is not a *complete* bipartite graph because there are vertices in one partition that are not [[Adjacent|adjacent]] to every vertex in the other. For example vertex 1 is not adjacent to vertex B. In fact, none of the vertices in the red/upper partition is connected to *all* vertices in the blue/lower one. 

The complete bipartite version of the graph above is denoted $K_{4,5}$ since there are 4 vertices in one partition and 5 in the other, and it looks like this (the vertices are relabeled and the graph is "sideways" but it is isomorphic to the first one): 

![[bipartite2.png|400]]

The complete bipartite graph $K_{3,3}$ is frequently encountered in discrete mathematics as an example or counterexample of different properties: 
![[k33-colored.png|400]]

For example, $K_{3,3}$ is one of the simplest examples of a non-[[Planar graph|planar]] graph. 

A very simple example of a graph that is *not* bipartite is $C_3$, the [[Cycle graph|cycle graph]] of length 3 which is just a triangle: 
![[k3.png|400]]

It is impossible to separate the vertices into two nonempty partitions in such a way that each edge has one endpoint in each partition. Any such partition must have one vertex in one set and the other two in the other, but the two in the second partition would be [[Adjacent|adjacent]]. 

In fact any graph that contains $C_3$ as a [[subgraph]] is automatically non-bipartite for the above reasons. In general, an even stronger statement can be made: 

> [!NOTE] Theorem
> A graph $G$ is bipartite if and only if it contains no [[Paths|cycle]] of [[Even and odd integers|odd]] length. 

## Resources 

![](https://www.youtube.com/watch?v=HqlUbSA9cEY)

