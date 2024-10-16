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
> 	b) Create a list of that node's [[Adjacent|neighbors]]. Add the ones which are not in the visited list $V$ to the "top" (or "right") of $S$. 
> 	
>The result of the algorithm is a list of vertices with a particular order of visiting. 


**Notes**: 
- The list $S$ is known in computer science and data structures as a [stack](https://www.geeksforgeeks.org/stack-data-structure/). This is a data structure in which operations are performed "first in, last out" or "last in, first out" -- the most recently added (or "rightmost", or "topmost") items are the ones removed first, like a stack of books or dinner plates. 
- The DFS algorithm is essentially the same as [[Breadth first search|breadth first search]] except in breadth first search, instead of a stack we use a [queue](https://www.geeksforgeeks.org/queue-data-structure/). 
- This is known as *depth first* search because it traverses the graph by moving as far in a single direction as possible before reaching a dead end, then it backtracks and recursively travels the other possible paths in the graph. 
- This is known as depth first *search* because the algorithm is often implemented with additional stopping conditions that halt the process once a node with a particular property is visited. 

## Examples 

(Taken from [this tutorial website](https://www.programiz.com/dsa/graph-dfs)) Consider the undirected graph below: 
![[dfs-image.png]]
Choose vertex 0 as the start point. We initialize $S = [0]$ and $V = [ \ ]$. Initially $S$ is nonempty, so: 
* Remove $0$ from $S$ and put it into the visited list: $V = [0]$. 
* Make a list of all of the [[Adjacent|neighbors]] of $0$: $1$, $2$, and $3$. None of these are in the visited list, so add them to the stack $S$: $S = [1,2,3]$. 
* Repeat the loop: The stack is nonempty, so remove the "top" item and add it to $V$: $V = [0,3]$. (And $S = [1,2]$.) Make a list of all the neighbors of 3: This time it's just 0, but that's already been visited. There are no new elements to add to $S$. 
* Repeat the loop: The stack is nonempty, so remove the top item and add it to $V$ to get $V = [0,3,2]$ and $S = [1]$. Make a list of all the neighbors of $2$: 0, 1, and 4. Of these, only 4 has not been visited yet, so add it to the stack: $S = [1,4]$. 
* Repeat the loop: The stack is nonempty, so remove the top item and add it to $V$ to get $V = [0,3,2, 4]$ and $S = [1]$. Make a list of all the neighbors of $4$: just 2. This is in the visited list, so there is nothing new to add to the stack. 
* Repeat the loop: The stack is nonempty, so remove the top item and add it to $V$ to get $V = [0,3,2, 4, 1]$ and $S = [ \ ]$. Make a list of all the neighbors of $1$: just 0 and 2. These are both in the visited list, so there is nothing to add to the stack. 
* The stack is now empty, so the algorithm stops and returns $V = [0,3,2,4,1]$. 
## Resources 

![](https://www.youtube.com/watch?v=7fujbpJ0LB4)

Other resources: 
- [Depth first search visualizer](https://www.cs.usfca.edu/~galles/visualization/DFS.html) (randomly generates a graph and animates the DFS process)
- [NetworkX DFS implementation docs](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.traversal.depth_first_search.dfs_edges.html#networkx.algorithms.traversal.depth_first_search.dfs_edges)
