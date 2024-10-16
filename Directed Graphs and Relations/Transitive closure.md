---
aliases:
  - transitive closure
tags:
  - digraphs-relations
created: 2024-10-16
updated:
---
---
## Definition 

> [!tldr] Definition
> Given a [[Directed graph|directed graph]] $G$, the **transitive closure** of $G$ is another directed graph denoted $G^+$  in which: 
> 1. The vertices are the same as those of $G$, and 
> 2. Given two vertices $a$ and $b$, there is a directed edge $(a,b)$ in $G^+$ if there is a directed [[Paths|path]] from $a$ to $b$ in the original digraph $G$.  

Notes: 
- The transitive closure of a digraph automatically includes all the existing edges in the original digraph, because if there is a directed edge from $a$ to $b$ then this is a directed path of length 1. 
- In the context of a social network in which the connections are directed (like Twitter, where "following" can be one-directional), there would be an edge from one user to another if there is a chain of followers that starts with the first user and ends with the second. 

## Examples 

Consider this directed graph: 
![[tc-graphic.png]]
The transitive closure of this graph would include all six vertices and all eight of the existing edges, but would add an edge between any two vertices that have a directed path connecting them. These edges would include: 
- $(4,5)$: There is no edge from 4 to 5 in the original, but there is a directed path from 4 to 5 -- the sequence 4, 3, 5. So in the transitive closure we would connect 4 to 5 directly. 
- 



There is no edge from 4 to 5 in this graph. However, there is a directed path starting at 4 and ending at 5, namely the sequence 4, 3, 5. So in the transitive closu

## Resources 

(video)

Other resources: 
- 

## Practice 
