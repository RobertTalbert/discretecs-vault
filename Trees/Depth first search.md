---
aliases:
  - DFS
  - depth first search
tags:
  - tree-search
created: 2024-10-16
updated:
---
---
## Definition 

> [!tldr] Definition
> **Depth first search** is an algorithm for visiting the nodes of a [[Graph|graph]] in a particular order. Given a graph $G$ and a starting vertex $a$, the algorithm proceeds as follows: 
> 
> 1. Initialize a list $S$ of nodes, initially consisting just of the start node $a$; and another list $V$ of visited nodes which is initially empty. 
> 2. While $S$ is nonempty:
> 	a) Take the top item from $S$ -- that is, the last or "rightmost" item added -- and remove it from the list and add it to $V$, the list of visited nodes. 
> 	b) Create a list of that node's neighbors. Add the ones which are not in the visited list $V$ to the "top" (or "right") of $S$. 
> 	
>The result of the algorithm is a list of vertices with a particular order of visiting. 


**Notes**: 
- The list $S$ is known in computer science and data structures as a [stack](https://www.geeksforgeeks.org/stack-data-structure/). This is a data structure in which operations are performed "first in, last out" or "last in, first out" -- the most recently added (or "rightmost", or "topmost") items are the ones removed first. 
- This is known as depth first *search* because the algorithm is often implemented with additional stopping conditions that halt the process once a node with a particular property is visited. 

## Examples 

(Taken from [this tutorial website](https://www.programiz.com/dsa/graph-dfs)) Consider the undirected graph below: 


## Resources 

(video)

Other resources: 
- [Depth first search visualizer](https://www.cs.usfca.edu/~galles/visualization/DFS.html) (randomly generates a graph and animates the DFS process)

## Practice 
