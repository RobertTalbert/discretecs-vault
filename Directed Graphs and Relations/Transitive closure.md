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

**Notes**: 
- The transitive closure of a digraph automatically includes all the existing edges in the original digraph, because if there is a directed edge from $a$ to $b$ then this is a directed path of length 1. 
- In the context of a social network in which the connections are directed (like Twitter, where "following" can be one-directional), there would be an edge from one user to another if there is a chain of followers that starts with the first user and ends with the second. 

## Examples 

Consider this directed graph: 
![[tc-graphic.png]]
The transitive closure of this graph would include all six vertices and all eight of the existing edges, but would add an edge between any two vertices that have a directed path connecting them. These edges would include: 
- $(4,5)$: There is no edge from 4 to 5 in the original, but there is a directed path from 4 to 5 -- the sequence 4, 3, 5. So in the transitive closure we would connect 4 to 5 directly. 
- $(6,2)$: There is no edge from 6 to 2 in the original, but there is a directed path from 6 to 2 -- the sequence 6, 1, 2. 
- The loops $(1,1)$ and $(2,2)$ because there is a directed path from 1 to itself (1, 2, 1) and likewise there is a directed path from 2 to itself. 
- $(2,5)$: There is a directed path 2, 1, 5 (also 2, 1, 3, 5). 

There are more edges than just these. The completed transitive closure looks like the following. Note, the loops are not shown due to limitations on the graphing software being used. There are only two self-loops, on vertices 1 and 2. 

![[tc-graph2.png]]


## Resources 

![](https://www.youtube.com/watch?v=OO8Jfs9uZnc)

Note, this video refers to the transitive closure of a [[Relation|relation]], not of a directed graph; however every directed graph is a relation and vice versa so the two terms can be used interchangeably. Also, the video uses $r^*$ rather than $r^+$ to denote the transitive closure. 