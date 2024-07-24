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
> A [[Graph|graph]] $G = (V,E)$ is **bipartite** if we can partition the [[Graph|vertex]] set $V$ into two nonempty [[Set|sets]], say $X$ and $Y$, such that every [[Graph|edge]] of the graph has exactly one [[Graph|endpoint]] in $X$ and one endpoint in $Y$. 
> 
> A bipartite graph in which each vertex in one of the partitions is [[Adjacent|adjacent]] to *every* vertex in the other partition, is called a **complete bipartite graph**. For a complete bipartite graph, if one of the partitions has $n$ vertices and the other has $m$, we denote it $K_{n,m}$. 

Notes: 
- 

## Examples

The graph below is bipartite, with the partitions separated into red/numbers and blue/letters: 
![[bipartite1.png]]
It is bipartite because every edge has one endpoint in one of the partitions and the other endpoint in the other partition. However it is not a *complete* bipartite graph because there are vertices in one partition that are not [[Adjacent|adjacent]] to every vertex in the other. For example vertex 1 is not adjacent to vertex B. In fact, none of the vertices in the red/upper partition is connected to *all* vertices in the blue/lower one


## Resources 

(video)

Other resources: 
- 

## Practice 
