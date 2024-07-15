---
aliases:
  - path, paths, walk, Walk, walks, cycle, Cycle, cycles, trail, Trail
tags:
  - graphs
created: 2024-07-15
updated:
---
---
## Definition 

> [!tldr] Definition
> Given a [[Graph|graph]] $G = (V,E)$:
> 1. A **walk** is a nonempty, alternating sequence of vertices and edges that starts and ends with a vertex, and in which every edge in the sequence is preceded and succeeded by its endpoints. If the walk starts and ends with the same vertex, it is called a **closed walk**. 
> 2. A **trail** is a walk with no repeated edge. If the trail starts and ends with the same vertex, it is called a **closed trail** or **circuit**. 
> 3. A **path** is a trail with no repeated vertex. A path consisting of a single vertex is called a **trivial path**. 
> 4. A **cycle** is a closed trail that has at least three (3) different vertices in it, and the only repeating vertices are the first and the last. 
> 5. The **length** of a walk, trail, path, or cycle is the number of edges it contains. 

**Notes**: 
- Since we do not allow for loops or multiple edges in graphs, we typically represent walks, trails, paths, and cycles using only vertices. 

## Examples and Non-Examples

Consider this graph $G$: 
![[degree-graph-example.png]]


- The vertex sequence 4, 3, 2, 5, 3, 2 is a walk. But it is not a trail, because it has a repeated edge (3,2). Since it is not a trail, it is also not a path. 
- The vertex sequence 4, 3, 2, 1, 3 is a walk, and also a trail because no edges are repeated. However it is not a path because there is a repeated vertex (3). 
- The vertex sequence 4, 3, 2, 6, 5 is a walk, a trail, and a path. But it is not a closed walk, closed trail, or cycle because the starting and ending vertices are not the same. 
- The vertex sequence 4, 3, 2, 3, 4 is a closed walk because it is a walk and it starts and ends at the same vertex. But is it not a trail (repeated edge) nor a path (repeated vertex), hence neither a closed trail nor a cycle. 
- There are in fact no cycles in this graph that start and end at 4. 
- However, the sequence 3, 1, 2, 6, 5, 3 is a cycle. 

The lengths of each of these is as follows:

| Vertex sequence | Length |     |
| --------------- | ------ | --- |
| 4,3,2,5,3,2     |        |     |
| 4,3,1,2,3       |        |     |
| 4,3,2,6,5       |        |     |
| 4,3,2,3,4       |        |     |
|                 |        |     |
 
## Resources 

(video)

Other resources: 
- 

## Practice 
