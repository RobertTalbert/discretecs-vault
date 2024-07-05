---
aliases:
  - adjacent
  - incident
  - neighbor
  - neighbors
tags: 
created: 2024-07-05
updated:
---
---
## Definition 

> [!tldr] Definition
> Two [[Graph|vertices]] $v$ and $w$ in a [[graph]] are said to be **adjacent** if they are the endpoints of an [[Graph|edge]]. We also say that $v$ and $w$ are **neighbors**. 
> 
> An [[Graph|edge]] in a graph is **incident** to a vertex if that vertex is one of its endpoints. Two edges are said to be **incident** to each other if they have an endpoint in common. 

Notes: 
- The word "incident" has two different uses: One to describe the relationship of an edge to a vertex, and another to describe the relationship between two edges. Be sure to be clear on the context when using that term.

## Examples and Non-Examples

Consider this graph: 
![[degree-graph-example.png]]
In this graph:
- Vertices $1$ and $2$ are adjacent. So are vertices $2$ and $6$. But vertex $1$ is *not* adjacent to vertex $6$. 
- The complete list of neighbors of vertex $3$ is: $1,2,4,5$. Vertex $3$ is adjacent to all of these. But it is not adjacent to vertex $6$. 
- The edge $\{2,5\}$ is incident to vertices $2$ and $5$. In fact every edge is incident to its two endpoints -- and to no other vertices. 
- The edges $\{2,5\}$ and $\{5,6\}$ are incident with each other. But $\{2,5\}$ is not incident with $\{1,3\}$. 
