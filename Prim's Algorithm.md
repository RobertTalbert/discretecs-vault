---
aliases: 
tags:
  - tree-search
created: 2024-10-02
updated:
---
---
## Definition 

> [!tldr] Definition
> **Prim's Algorithm** is an algorithm for constructing a [[Minimum spanning tree|minimum spanning tree]] inside a [[Weighted graph|weighted graph]]. If the graph is unweighted, then Prim's Algorithm will simply build a [[Documents/Graphs/Spanning tree|spanning tree]]. 
> 
> The algorithm works as follows. The input is a [[Connected graph|connected]], [[Weighted graph|weighted graph]] $G$. 
> 1. Choose an arbitrary vertex $v$ in $G$ and make this the first vertex in the spanning tree.
> 2. Look at all edges that go out from the tree. Choose an edge with the lowest weight that connects a vertex in the tree to a vertex outside the tree.
> 3. Add this edge and the new endpoint to the spanning tree. 
> 4. Repeat steps 2 and 3 until all vertices are in the spanning tree. 
>

Notes: 
- Prim's algorithm is an example of a greedy algorithm since it chooses the minimum weight edge each time. This will guarantee that the spanning tree is minimal. 
- The result of the algorithm is a tree since we are intentionally adding edges that do not create cycles. (In step 2 the algorithm adds an edge only if one endpoint is in the tree and the other is not, so no cycle is created.)

## Examples 

Consider this weighted graph: 
![[weighted.png]]
Prim's Algorithm starting at vertex 1 would proceed as follows: 
- Make 1 the first vertex in the tree. At this stage the tree is just this one vertex. 
- The edges that go out from "the tree" are 


## Resources 

(video)

Other resources: 
- 

## Practice 
