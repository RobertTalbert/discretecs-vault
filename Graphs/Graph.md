---
aliases:
  - graph
  - graphs
  - edge
  - edges
  - vertex
  - vertices
  - node
  - nodes
  - Graphs
  - Edge
  - Vertex
  - Node
  - Edges
  - Vertices
  - Nodes
tags:
  - graphs
created: 2024-07-01
updated:
---
---
## Definition 

> [!tldr] Definition
> A **graph** is a pair of [[Set|sets]]: 
> 1. A nonempty set called the **vertex set**, whose elements we call **vertices** or **nodes**. 
> 2. A (possibly empty) set called the **edge set**, whose elements we call **edges**, where each edge is a [[Subset|subset]] of the vertex set that contains exactly two elements (called the **endpoints** of the edge). 
>    
>  We often use $G = (V,E)$ to denote a graph whose name is $G$, whose vertex set is $V$, and whose edge set is $E$. 

Notes: 
- The definition of a graph is rather abstract because we want room to represent graphs in different ways: both visually, and as pure data structures in several different forms. 
- Note that the edge set of a graph is a set, whose elements are also sets -- namely, two-element subsets of the vertices. 


## Examples and Non-Examples

- Consider the graph $G = (\{a,b,c,d\}, \{\{a,c\}, \{a,d\}, \{d,c\}, \{a,b\}\})$. Note that this is a pair of sets, enclosed in parentheses. The first element of the pair is the set $\{a,b,c,d\}$, and these are the vertices. The second element is $\{\{a,c\}, \{a,d\}, \{d,c\}, \{a,b\}\}$ and these are the edges. There are four edges: One with endpoints $a$ and $c$; one with endpoints $a$ and $d$; a third with endpoints $d$ and $c$; and a fourth with endpoints $a$ and $b$. Note that because the edges are given as sets, not as ordered pairs, each edge is the same no matter what order we list the endpoints in. A visualization of the graph $G$ is: 
![[Pasted image 20240701115858.png|400]]

- When visualized in this way -- with each vertex shown as a point and each edge shown as a line segment between its endpoints -- graphs are representations of *networks*. 
- Consider the following visualization of a graph: 


This graph is $G = 


## Resources 

(video)

Other resources: 
- 

## Practice 
