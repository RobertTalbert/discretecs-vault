---
aliases:
  - directed graph
  - digraph
  - Digraph
  - digraphs
tags:
  - digraphs-relations
created: 2024-08-07
updated: 2024-10-21
---
---
## Definition 

> [!tldr] Definition
> A **directed graph** (or **digraph**) is pair of sets: 
> 1. A nonempty [set](app://obsidian.md/set) called the **vertex set**, whose elements we call **vertices** or **nodes**.
> 2. A (possibly empty) set called the **edge set**, whose elements we call **edges**, where each edge is an [[Cartesian product|ordered pair]] of vertices. 
> 
> We often use $G = (V,E)$ to denote a digraph whose name is $G$ with vertex set $V$ and edge set $E$. Note that $E$ is a [[Subset|subset]] of the [[Cartesian product]] $V \times V$. If $(u,v)$ is an edge in $G$, then we say that the edge **points from $u$ to $v$** and that $u$ is the **head** of the edge and $v$ is the **tail**. An edge of the form $(u,u)$ is called a **loop**. 

Notes: 
- Unlike a regular, undirected [[graph]], the edges of a digraph are *not* simply two-element subsets of the vertex set: They are *ordered pairs*. It is possible for $(u,v)$ to be an edge in a digraph but $(v,u)$ is not an edge. 
- We think of edges in a digraph as being vectors or arrows with a head and a tail. Sometimes we write $u \rightarrow v$ to represent an edge from $u$ to $v$. 

## Examples

Consider the digraph $G$ below: 

![[digraph-example.png|500]]

The vertex set of $G$ is $V = \{1,2,3,4,5\}$. The edge set is the following set of ordered pairs: 
$$E = \{(1,3), (2,1), (2,3), (2,5), (4,3)\}$$
Notice that although $(1,3)$ is an edge, $(3,1)$ is not. This is a *directed* graph and the ordering reflects the direction of the edge. 

Conversely, consider the digraph whose vertex set is $\{1,2,3,4\}$ and whose edge set is $E = \{(1,2), (1,3), (1,4), (3,2), (3,4), (4,2), (4,3)\}$. As a visual diagram, $G$ looks like: 

![[digraph-example2.png|400]]
This digraph has no loops, but it does have two vertices (3 and 4) with edges pointing in both directions. 

## Resources 

![](https://www.youtube.com/watch?v=mXoiHgH4mEE)

