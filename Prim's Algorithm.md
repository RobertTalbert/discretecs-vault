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
- The edges that go out from "the tree" are $\{1,7\}$ and $\{1,0\}$. Of those, the one with minimum weight is $\{1,0\}$. It connects a vertex in the tree (1) with one that is not (0) so add this edge to the tree. The tree is now the single edge $\{0,1\}$. 
- The tree does not contain all the vertices yet, so look at all edges that come out from the tree with one vertex in the tree and the other not in the tree: $\{0,3\}, \{0,8\},$ and $\{1,7\}$. The one with lowest weight is $\{0,3\}$. It connects a vertex in the tree with one outside the tree, so add it to the tree. The tree is now $\{\{0,1\}, \{0,3\}\}$. 
- The tree does not contain all the vertices yet, so look at all edges that come out from the tree with one vertex in the tree and the other not in the tree: $\{0,8\},\{3,4\}, \{3,2\}$ and $\{1,7\}$. The edge with the lowest weight is $\{3,4\}$ and it connects a vertex in the tree with one not in the tree, so add it to the tree: $\{\{0,1\}, \{0,3\}, \{3,4\}\}$. 
- Look at all edges that come out from the tree with one vertex in the tree and the other not in the tree: $\{0,8\},\{4,8\},\{3,2\}$ and $\{1,7\}$. There's a tie for lowest weight between $\{0,8\}$ and $\{1,7\}$ so choose one, let's say $\{0,8\}$, and add it: : $\{\{0,1\}, \{0,3\}, \{3,4\}, \{0,8\}\}$. 
- Look at all edges that come out from the tree with one vertex in the tree and the other not in the tree: $\{1,7\}$ and $\{3,2\}$. Note, we would *not* look at $\{4,8\}$ this time even though we considered it earlier, because it no longer connects a vertex in the tree with one outside the tree -- that means adding it would create a cycle. Of the two eligible edges, $\{1,7\}


## Resources 

(video)

Other resources: 
- 

## Practice 
