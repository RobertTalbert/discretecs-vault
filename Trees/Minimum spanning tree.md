---
aliases:
  - minimum spanning tree
tags:
  - tree-search
created: 2024-10-02
updated:
---
---
## Definition 

> [!tldr] Definition
> Given a [[Weighted graph|weighted graph]] $G$, a **minimum spanning tree** is a [[Spanning tree|spanning tree]] such that the sum of the edge weights is the smallest of all spanning trees of $G$. 

Notes: 
- It is possible for a [[Weighted graph|weighted graph]] to have more than one minimum spanning tree, that is, more than one [[Spanning tree|spanning tree]] having the same minimum edge weight sum. But, there can only be one minimum edge weight sum. 

## Examples 

Consider this weighted graph: 
![[weighted.png]]
There are several spanning trees for this graph, including: 
* $\{\{0,1\}, \{0,3\}, \{3,4\}, \{0,8\}, \{1,7\}, \{2,7\}, \{2,5\}, \{5,6\}\}$
* $\{\{4,8\}, \{8,0\}, \{0,3\}, \{0,1\}, \{3,2\}, \{1,7\}, \{2,5\}, \{5,6\}\}$

But notice that the weights are different. The total weight of the first spanning tree is $4+3+4+2+2+1+1+8 = 25$ while the second is $8+4+2+3+6+4+1+8 = 36$. In fact the first tree is a *minimal* spanning tree, because there is no other spanning tree with a lower total weight. It was constructed using [[Prim's Algorithm]], an algorithm that guarantees a minimum spanning tree as an output. 
## Resources 

![](https://www.youtube.com/watch?v=Yldkh0aOEcg)
