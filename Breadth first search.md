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
> 	a) Take the front item from $Q$ -- that is, the first or "leftmost" item -- and remove it from the list and add it to $V$, the list of visited nodes. 
> 	b) Create a list of that node's [[Adjacent|neighbors]]. Add the ones which are not in the visited list $V$ to the "bottom" (or "left") of $S$. 
> 	
>The result of the algorithm is a list of vertices with a particular order of visiting. 

**Notes:**
- The list $Q$ is known in computer science and data structures as a [queue](https://www.geeksforgeeks.org/queue-data-structure/). This is a data structure in which operations are performed "first in, first out" or "last in, last out" -- the most recently added (or "rightmost", or "topmost") items are the ones removed last. It works like a waiting line ([the literal use of the word "queue"](https://www.merriam-webster.com/dictionary/queue)). 
- The BFS algorithm is essentially the same as [[Depth first search|depth first search]] except in depth first search, instead of a queue we use a [stack](https://www.geeksforgeeks.org/stack-data-structure/). 
- This is known as *breadth first* search because it traverses the graph by moving out "one level at a time" and gradually proceeding through the graph after all the nearby vertices are visited. 
- This is known as depth first *search* because the algorithm is often implemented with additional stopping conditions that halt the process once a node with a particular property is visited. 

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 
