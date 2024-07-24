---
aliases:
  - coloring
  - vertex coloring
  - graph coloring
  - color
  - colorings
tags:
  - graphs
created: 2024-07-24
updated:
---
---
## Definition 

> [!tldr] Definition
> Given a [[Graph|graph]] $G$, a **vertex coloring** (or just a **coloring**) is a [[Function|function]] that assigns to each vertex of $G$ some label that we will call a **color**. A **proper vertex coloring** (or just a **proper coloring**) is a vertex coloring of $G$ in which adjacent [[Graph|vertices]] receive different colors; that is, if two vertices have the same color, they cannot be adjacent (and vice versa). A proper coloring that contains $n$ colors is said to be an $n$-coloring of the graph; a graph that has an $n$-coloring is said to be $n$-colorable. 

Notes: 
- The labels used in a coloring are not necessarily literally colors; they can be text labels, numbers, etc. 
- Every graph has a proper coloring, which can be obtained by using a different color for every vertex. 

## Examples and Non-Examples

**An improper vertex coloring:** The graph below has ten vertices labelled 1 through 10 and colored red, green or blue:

![[improper-coloring.png|400]]

The coloring, given as a function $f$, could be represented as this table: 

|  $v$   | 1   | 2   | 3   | 4   | 5   | 6   | 7    | 8    | 9    | 10    |
| :----: | --- | --- | --- | --- | --- | --- | ---- | ---- | ---- | ----- |
| $f(v)$ | Red | Red | Red | Red | Red | Red | Blue | Blue | Blue | Green |
 
(This is not the only way to represent a coloring.) Note **this is not a proper coloring** because for example, vertices 1 and 2 are adjacent but have the same color. 

**A proper coloring:** An example of a *proper* coloring of the graph above -- where adjacent vertices have different colors -- is below, where 1 is red, the remaining odd numbered vertices are blue, and the even numbered vertices are green: ![[proper-coloring.png|400]]

As noted, another example of a proper coloring of this graph can be created by simply coloring each vertex with a different color, so 10 colors in all. But this would use more colors than is necessary; typically, in applications, we are seeking the smallest number of colors needed to create a proper coloring of a graph, a concept related to the [[Chromatic number|chromatic number]] of the graph. 

More examples: 
- 

## Resources 

![](https://www.youtube.com/watch?v=3VeQhNF5-rE)

