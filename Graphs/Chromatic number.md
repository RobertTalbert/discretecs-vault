---
aliases:
  - chromatic number
tags:
  - graphs
created: 2024-07-24
updated:
---
---
## Definition 

> [!tldr] Definition
> The **chromatic number** of a graph $G$ is the minimum number of colors in any proper [[Vertex coloring|vertex coloring]] of $G$. The chromatic number of $G$ is denoted $\chi(G)$. 

Notes
- $\chi$ is the Greek letter "chi", pronounced "Kie" (rhymes with "pie"). 
- A given graph can have many different possible proper [[Vertex coloring|colorings]]; for example we can just assign a different color to each vertex. But there is only one minimum number of colors needed for a proper coloring, and that number is $\chi(G)$. 

## Examples 

The chromatic number of $K_3$, the [[Complete graph|complete graph]] on three vertices, is $3$. Since each vertex is adjacent to the other two, three colors are necessary for a proper coloring, and two colors are not enough: 
![[colored-k3.png|400]]

By extension, $\chi(K_n) = n$ (where $K_n$ is the [[Complete graph|complete graph]] on $n$ vertices) for every positive [[Integers|integer]] $n$, since each vertex is adjacent to the remaining $n-1$ vertices. 

Also by extension, any graph that has $K_3$ (a triangle) as a [[Subgraph|subgraph]] must have a chromatic number greater than or equal to 3, since a minimum of 3 colors is required to color just the triangle. 





## Resources 

(video)

Other resources: 
- 

## Practice 
