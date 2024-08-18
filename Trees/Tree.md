---
aliases:
  - tree
  - trees
  - Trees
  - forest
  - Forest
tags:
  - tree-search
created: 2024-07-30
updated: 2024-08-09
---
---
## Definition 

> [!tldr] Definition
> A **tree** is a [[graph]] which is [[Connected graph|connected]] and which contains no [[Paths|cycles]]. 

Notes: 
- A collection of trees is called a **forest**. That is, a forest is a [[graph]] that has no [[Paths|cycles]] (but which might be disconnected). 
- In a tree, there is a unique path between any two vertices. That is, given any two vertices, there exists a path from one to the other; and only one such path exists. 

## Examples 

An example of a tree: 
![[tree-example1.png|100]]

Another example: 

![[tree-example2.png|400]]

Each of the [[Graph|graphs]] below is a tree, used to model molecular structure in chemistry: 
![[tree-example3.png]]

This [[graph]] below on the left is not a tree, because it contains a [[Paths|cycle]] ([source](https://www.gatevidyalay.com/tree-data-structure-tree-terminology/)): 

![[tree-example4.png]]

The image below, taken to be a single [[graph]] with three [[Connected graph|components]], is not a tree, because it is not [[Connected graph|connected]]. But, we can think of it as a forest. 

![[tree-example5.png]]


## Resources 

![](https://www.youtube.com/watch?v=QFQlxtz7f6g)

![](https://www.youtube.com/watch?v=BptJFixSseM)