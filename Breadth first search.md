---
aliases:
  - BFS
  - breadth first search
tags:
  - tree-search
created: 2024-10-16
updated:
---
---
## Definition 

> [!tldr] Definition
> **Breadth first search** is an algorithm for visiting the nodes of a [[Graph|graph]] in a particular order. Given a graph $G$ and a starting vertex $a$, the algorithm proceeds as follows: 
> 
> 1. Initialize a list $Q$ of nodes, initially consisting just of the start node $a$; and another list $V$ of visited nodes which is initially empty. 
> 2. While $Q$ is nonempty:
> 	a) Take the bottom item from $Q$ -- that is, the first or "leftmost" item added -- and remove it from the list and add it to $V$, the list of visited nodes. 
> 	b) Create a list of that node's [[Adjacent|neighbors]]. Add the ones which are not in the visited list $V$ to the "bottom" (or "left") of $S$. 
> 	
>The result of the algorithm is a list of vertices with a particular order of visiting. 

(blurb)

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 
