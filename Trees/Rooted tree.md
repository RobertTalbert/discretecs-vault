---
aliases:
  - rooted tree
  - root
  - Root
  - leaf
  - Leaf
  - leaves
  - parent
  - child
  - height
  - depth
  - Depth
tags:
  - tree-search
created: 2024-08-09
updated:
---
---
## Definition 

> [!tldr] Definition
> A **rooted tree** is a labelled [[Tree|tree]] in which one specific [[Graph|vertex]] is marked as being "special". That [[Graph|vertex]] is called the **root**. 
> 
>If $v$ is a [[Graph|vertex]] in a rooted tree that has [[Degree|degree]] equal to 1, we say that the vertex is a **leaf** of the tree. The **height** a rooted tree is the length of the longest path from the root to a leaf. The **depth** of a vertex is the length of the (unique) path from that vertex to the root; the depth of the tree itself is the maximum depth of any vertex. 
> 
> If $u$ and $v$ are vertices in a rooted tree, we say that $u$ is the **parent** of $v$ if $u$ is a [[Adjacent|neighbor]] of $v$, and $u$ is closer to the root than $v$ (in terms of the length of the path from the root to these vertices). If $u$ is the parent of $v$, then we say $v$ is a **child** of $u$. 

Notes: 
- In a visual diagram of a tree, we often put the root at the top of the tree (unlike a real-life tree!). 
- Note that although a vertex in a rooted tree can have multiple children, it can have no more than one parent. (If it had two parents, a cycle would be created, which is impossible in a tree.)

## Examples 

Consider the tree below whose root is 2: 
![[tree-example1.png|200]]

The leaves of this tree are the vertices 3, 7, and 8. The height of the tree is 4 (the length of the longest path from the root to a leaf.) The depth of vertex 4 is 3 (the length of the unique path from the vertex to the root) and the depth of the tree itself is 4. The parent of vertex 4 is 5, and vertex 4 has two children, 3 and 8. 

Another example: 
![[tree-example2.png]]
Again the root is 2. The leaves are (reading from left to right) 15, 8, 17, 1, 3, 5, 4, 9, 19, 6, and 16. The height of the tree is 4. The depth of vertex 12 is 3; the depth of vertex 5 is 1. The parent of vertex 19 is 14; and 19 has no children. 


## Resources 
![](https://www.youtube.com/watch?v=QFQlxtz7f6g)

