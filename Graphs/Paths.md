---
aliases:
  - path
  - paths
  - walk
  - Walk
  - walks
  - cycle
  - Cycle
  - cycles
  - trail
  - Trail
  - circuit
  - Circuit
tags:
  - graphs
created: 2024-07-15
updated:
---
---
## Definition 

> [!tldr] Definition
> Given a [[Graph|graph]] $G = (V,E)$:
> 1. A **walk** is a nonempty, alternating sequence of [[Graph|vertices]] and edges that starts and ends with a vertex, and in which every [[Graph|edge]] in the sequence is preceded and succeeded by its endpoints. If the walk starts and ends with the same vertex, it is called a **closed walk**. 
> 2. A **trail** is a walk with no repeated edge. If the trail starts and ends with the same vertex, it is called a **closed trail** or **circuit**. 
> 3. A **path** is a trail with no repeated vertex. A path consisting of a single vertex is called a **trivial path**. 
> 4. A **cycle** is a closed trail that has at least three (3) different vertices in it, and the only repeating vertices are the first and the last. 
> 5. The **length** of a walk, trail, path, or cycle is the number of edges it contains. 
>    
>    We often omit the edges from walks, trails, paths, and cycles and just list the vertices in a sequence. In this case a walk is a nonempty sequence of vertices in which any two consecutive vertices are [[Adjacent|adjacent]]. 

**Notes**: 
- Since we do not allow for loops or multiple edges in graphs, we typically represent walks, trails, paths, and cycles using only vertices. 
- There is no such thing as a closed trail or cycle of length 1 or 2; length 1 would mean that the starting and ending vertices are different, and length 2 would mean traversing the same edge twice. However it is possible to have a closed walk of length 2: On an edge $(a,b)$, the sequence $a,b,a$ would be a closed walk of length 2. 
- A cycle of length 3 is a triangle. 

## Examples and Non-Examples

Consider this graph $G$: 
![[degree-graph-example.png]]


- The vertex sequence 4, 3, 2, 5, 3, 2 is a walk because it's a nonempty sequence of vertices in which every pair of consec. But it is not a trail, because it has a repeated edge (3,2). Since it is not a trail, it is also not a path. 
- The vertex sequence 4, 3, 2, 1, 3 is a walk, and also a trail because no edges are repeated. However it is not a path because there is a repeated vertex (3). 
- The vertex sequence 4, 3, 2, 6, 5 is a walk, a trail, and a path. But it is not a closed walk, closed trail, or cycle because the starting and ending vertices are not the same. 
- The vertex sequence 4, 3, 2, 3, 4 is a closed walk because it is a walk and it starts and ends at the same vertex. But is it not a trail (repeated edge) nor a path (repeated vertex), hence neither a closed trail nor a cycle. 
- There are in fact no cycles in this graph that start and end at 4. 
- However, the sequence 3, 1, 2, 6, 5, 3 is a cycle. 
- The sequence 3, 2, 5, 3 is a cycle of length 3. 

The lengths of each of these is as follows:

| Vertex sequence | Length |
| --------------- | ------ |
| 4,3,2,5,3,2     | 5      |
| 4,3,1,2,3       | 4      |
| 4,3,2,6,5       | 4      |
| 4,3,2,3,4       | 4      |
| 3,1,2,6,5,3     | 5      |
| 3,2,5,3         | 3      |


## Resources 

![](https://www.youtube.com/watch?v=hlHWguJVAdU)
