---
aliases: spanning tree
tags: graphs
created: 2024-08-15
updated:
---
---
## Definition 

> [!tldr] Definition
> Let $G$ be a [[Graph|graph]]. A **spanning tree** of $G$ is a [[Subgraph|subgraph]] of $G$ that contains all the [[Graph|vertices]] of $G$ and is a [[tree]].  

Notes: 
- A spanning tree need not include all the [[Graph|edges]] of $G$; usually many edges are not included. 
- A [[Graph|graph]] can have more than one spanning tree; see below for examples. 


## Examples and Non-Examples

Let $G = K_4$, the [[complete graph]] on 4 vertices: 

![[k4-2.png|400]]

The [[subgraph]] whose vertices are $1,2,3,4$ and whose edges are $\{\{1,2\}, \{1,3\}, \{1,4\}\}$ is a spanning tree of $G$: 

![[k4-spanning.png|400]]

So is the graph whose vertices are $1,2,3,4$ and whose edges are $\{\{1,2\}, \{2,3\}, \{2,4\}\}$. 

But the subgraph whose vertices are $1,2,3,4$ and whose edges are $\{\{1,2\}, \{2,3\}, \{3,4\}, \{1,4\}\}$ is not a spanning tree, because although this subgraph contains all the vertices of $G$, it is not a tree because it has a cycle. (The entire subgraph is a cycle, in fact it is $C_4$, the [[cycle graph]] on four vertices.)

Neither is the subgraph whose vertices are $1,2,3$ and whose edges are $\{\{1,2\}, \{1,3\}\}$ because although this subgraph is a tree, it does not contain all the vertices of $G$. 


## Resources 

![](https://www.youtube.com/watch?v=fO-R1vwgsmw)