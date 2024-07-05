---
aliases:
  - degree
  - vertex degree
  - minimum degree
  - maximum degree
tags:
  - graphs
created: 2024-07-05
updated:
---
---
## Definition 

> [!tldr] Definition
> The **degree** of a vertex in a [[Graph|graph]] is the number of edges that are [[incident]] to $v$. That is, it is the number of edges "coming out" of the vertex. If $v$ is a specific vertex, then its degree is denoted $\deg(v)$.
> 
> The **minimum degree** of a graph $G$ is the smallest of all its vertex degrees and is denoted $\delta(G)$. The **maximum degree** of a graph $G$ is the smallest of all its vertex degrees and is denoted $\Delta(G)$.
> 
> The **degree sequence** of a graph is the list of all of its vertex degrees listed in non-increasing order. 



Notes: 
- If $G$ is the graph to which $v$ belongs as a vertex, we sometimes denote this by adding $G$ as a subscript: $\deg_G(v)$. 
- $\delta$ is the lower-case Greek letter "Delta". $\Delta$ is the upper-case form. 

## Examples 

Consider this graph: 
![[degree-graph-example.png]]

The degrees each vertex are: 

| Vertex |    Degree     |
| :----: | :-----------: |
|   1    | $\deg(1) = 2$ |
|   2    | $\deg(2) = 4$ |
|   3    | $\deg(3) = 4$ |
|   4    | $\deg(4) = 1$ |
|   5    | $\deg(5) = 3$ |
|   6    | $\deg(6) = 2$ |
And for this graph, $\delta(G) = 1$ and $\Delta(G) = 4$. 


## Resources 

![](https://www.youtube.com/watch?v=C4s5j2-Hos4)