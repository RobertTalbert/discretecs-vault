---
aliases:
  - subdivision
  - subdivisions
tags:
  - graphs
created: 2024-07-24
updated:
---
---
## Definition 

> [!tldr] Definition
> Suppose $G$ and $H$ are [[Graph|graphs]]. We say $H$ is a **subdivision** of $G$ if $H$ is obtained from $G$ by replacing [[Graph|edges]] of $G$ with [[Paths|paths]] of any lengths. The [[Graph|vertices]] of $H$ that correspond to directly to the vertices of $G$ are called **branch vertices**. 

Notes: 
- Visually, a graph $H$ is a subdivision of another graph $G$ if we take $G$ and add new vertices to it along existing edges, "splitting up" the edges with those vertices. 

## Example

Consider this graph $G$ with 4 vertices and 5 edges: 
![[subdivision1.png|400]]
Then this graph $H$ is a subdivision of $G$:
![[subdivision2.png|450]]
Here, we have replaced the edge $\{1,3\}$ with the path $1, v_5, 3$. Similarly there are new vertices in "the middle" of the other four original edges. The vertices 1,2,3,4 correspond directly to vertices in the original $G$ and are thus the branch vertices. 

## Resources 

![](https://www.youtube.com/watch?v=ciqdbjB_syM)

