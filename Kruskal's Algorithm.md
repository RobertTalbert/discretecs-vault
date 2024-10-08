---
aliases: 
tags:
  - tree-search
created: 2024-10-08
updated:
---
---
## Definition 

> [!tldr] Definition
> **Kruskal's Algorithm** is an algorithm for constructing a [[Minimum spanning tree|minimum spanning tree]] inside a [[Weighted graph|weighted graph]]. 
> 
> The algorithm works as follows. The input is a [[Connected graph|connected]], [[Weighted graph|weighted graph]] $G$. 
> 
> 1. Sort all of the edges of $G$ in non-decreasing order of weight and initialize an empty [[Tree|tree]] (that will eventually be a minimum spanning tree). 
> 2. Select an edge with minimum weight. Check if it forms a cycle if added to the tree. If it does, discard it. If it does not, add it to the tree. 
> 3. Repeat step 2 until the number of edges in the tree is one less than the number of vertices in $G$. 

Notes: 
- [[Prim's Algorithm]] is a different approach that also finds a minimum spanning tree -- not necessarily the same tree as found by Prim's Algorithm but the total weight will be the same. 
- Kruskal's Algorithm produces a graph with no cycles due to step 2's instructions. The end result is a tree because a graph that has no cycles and whose number of edges is one less than the number of vertices, must be a tree. 

## Example

Consider this weighted graph: 
![[weighted.png]]

Sort the edges in non-decreasing order of weight: 

$$\{2,5\}, \{3,4\}, \{0,3\}, \{2,7\}, \{0,1\}, \{0,8\}, \{1,7\}, \{3,2\}, \{8,4\}, \{5,6\}\}$$

Initialize $T$ to be the empty tree. 

- There are two edges with lowest weight (equal to 1), so just pick one: $\{2,5\}$. The current tree is empty so adding this edge does not produce a cycle. The tree becomes $\{\{2,5\}\}$. 
- Repeat this step: The next edge of smallest weight is $\{3,4\}$. Adding it to the tree does not create a cycle, so add it to get  $T = \{\{2,5\}, \{3,4\}\}$. (Note, )

## Resources 

(video)

Other resources: 
- 

## Practice 
