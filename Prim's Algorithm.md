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
> 2. Look at all edges that go out from the tree. Choose an edge with the lowest weight that connects a vertex in the tree to a vertex outside the tree, and which will not form a cycle if added into the spanning tree.
> 3. Add this edge and the new endpoint to the spanning tree. 
> 4. Repeat steps 2 an

(blurb)

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 
