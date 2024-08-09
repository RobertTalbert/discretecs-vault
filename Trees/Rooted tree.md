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
>If $v$ is a [[Graph|vertex]] in a rooted tree that has [[Degree|degree]] equal to 1, we say that the vertex is a **leaf** of the tree. The **height** of a vertex in a tree, is the length of the longest [[Paths|path]] to a leaf from that vertex. The **height** of the tree itself, is defined to be the height of the root. The **depth** of a vertex is the length of the (unique) path from that vertex to the root; the depth of the tree itself is the maximum depth of any vertex. 
> 
> If $u$ and $v$ are vertices in a rooted tree, we say that $u$ is the **parent** of $v$ if $u$ is a [[Adjacent|neighbor]] of $v$, and $u$ is closer to the root than $v$ (in terms of the length of the path from the root to these vertices). If $u$ is the parent of $v$, then we say $v$ is a **child** of $u$. 

Notes: 
- In a visual diagram of a tree, we often put the root at the top of the tree (unlike a real-life tree!). 

## Examples 

Consider the tree below whose root is 2: 
![[tree-example1.png|200]]

The leaves of this tree are the vertices 3, 7, and 8. The height of vertex 4 is the length of the longest path 

## Resources 

(video)

Other resources: 
- 

## Practice 
