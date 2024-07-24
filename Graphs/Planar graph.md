---
aliases:
  - planar
  - planar graph
  - Planar
tags:
  - graphs
created: 2024-07-24
updated:
---
---
## Definition 

> [!tldr] Definition
> A [[Graph|graph]] is said to be **planar** if it can be drawn in a plane (for example, on one side of a flat piece of paper) in such a way that no two [[Graph|edges]] intersect, with the only exception being that [[Adjacent|incident]] edges intersect exactly once at their common [[Graph|vertex]]. Such a drawing is called a **planar representation** of the graph. A graph that has no planar representation is called **nonplanar**. 

Notes: 
- A graph is planar if it is *possible* to draw a planar representation. Sometimes graphs may appear at first to be nonplanar but a careful redrawing can remove intersecting edges. 

## Examples and Non-Examples

The [[Complete graph|complete graph]] on 4 vertices, $K_4$, *appears* to be nonplanar in this visualization because of the two intersecting edges in the middle: 
![[k4-nonplanar.png|400]]
But in fact this graph *is* planar, because it is possible to redraw it in a way that has no intersecting edges: 
![[k4.png|400]]

On the other hand, $K_5$ is nonplanar: 
![[k5.png|400]]

It is impossible to redraw $K_5$ without edge crossings due to [[Kuratowski's Theorem]] which states in part that if a graph contains $K_5$ or a subdivision of $K_5$ as a [[Subgraph|subgraph]] then the graph is nonplanar. 

## Resources 

![](https://www.youtube.com/watch?v=wnYtITkWAYA)

