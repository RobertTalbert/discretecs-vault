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

## Resources 

(video)

Other resources: 
- 

## Practice 
