---
aliases:
  - edge coloring
  - chromatic index
  - Chromatic index
tags:
  - graphs
created: 2024-07-24
updated:
---
---
## Definition 

> [!tldr] Definition
> Given a [[Graph|graph]] $G$, an **edge coloring** of $G$ is a function that assigns to every [[Graph|edge]] of $G$ some label. A **proper edge coloring** is an edge coloring in which [[Adjacent|incident]] edges receive different colors; that is, if two edges have the same color, they cannot be incident (and vice versa). 

Notes: 
- The labels used in a coloring are not necessarily literally colors; they can be text labels, numbers, etc. 
- Every graph has a proper edge coloring, which can be obtained by using a different color for every edge. 

## Examples and Non-Examples

Here is a proper edge coloring of $K_4$ (the [[Complete graph|complete graph]] on 4 vertices):
![[k4-edge-color.png|400]]
This coloring uses six different colors, one for each edge. We can create a proper edge coloring with fewer colors, for example this one which uses only three edge colors: 
![[k4-edge-color-3.png|400]]


Here is an edge coloring of $K_4$ that is *not* proper, because the edges $\{1,2\}$ and $\{2,3\}$ have the same color even though they are incident: 
![[k4-improper-edge-color.png|400]]


## Resources 

![](https://www.youtube.com/watch?v=X2B_J1ajsIY)
