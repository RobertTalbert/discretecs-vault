---
aliases:
  - degree
  - vertex degree
  - minimum degree
  - maximum degree
  - degree sequence
  - degrees
tags:
  - graphs
created: 2024-07-05
updated:
---
---
## Definition 

> [!tldr] Definition
> The **degree** of a [[Graph|vertex]] in a [[Graph|graph]] is the number of [[Graph|edges]] that are [[Adjacent|incident]] to $v$. That is, it is the number of edges "coming out" of the vertex. If $v$ is a specific vertex, then its degree is denoted $\deg(v)$.
> 
> The **minimum degree** of a graph $G$ is the smallest of all its vertex degrees and is denoted $\delta(G)$. The **maximum degree** of a graph $G$ is the largest of all its vertex degrees and is denoted $\Delta(G)$.
> 
> The **degree sequence** of a graph is the list of all of its vertex degrees listed in non-increasing order. 



Notes: 
- If $G$ is the graph to which $v$ belongs as a vertex, we sometimes denote this by adding $G$ as a subscript: $\deg_G(v)$. 
- $\delta$ is the lower-case Greek letter "Delta". $\Delta$ is the upper-case form. 
- In the degree sequence for a graph $G$, $\Delta(G)$ is always the first number in the list and $\delta(G)$ is the last number. 

## Examples 

- Consider this graph: 
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
And for this graph, $\delta(G) = 1$ and $\Delta(G) = 4$, and the degree sequence is: $4,4,3,2,2,1$. 

- Here is another graph: 
![[degree-example-2.png]]

The individual vertex degrees are 

| Vertex |    Degree     |
| :----: | :-----------: |
|   1    | $\deg(1) = 6$ |
|   2    | $\deg(2) = 2$ |
|   3    | $\deg(3) = 3$ |
|   4    | $\deg(4) = 4$ |
|   5    | $\deg(5) = 4$ |
|   6    | $\deg(6) = 3$ |
|   7    | $\deg(7) = 6$ |
|   8    | $\deg(8) = 4$ |
The degree sequence is $6,6,4,4,4,3,3,2$, and we have $\Delta(G) = 6$ and $\delta(G) = 2$. 

## Resources 

![](https://www.youtube.com/watch?v=C4s5j2-Hos4)