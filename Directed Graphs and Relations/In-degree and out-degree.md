---
aliases:
  - in-degree
  - out-degree
  - In-degree
  - Out-degree
tags:
  - digraphs-relations
created: 2024-08-07
updated:
---
---
## Definition 

> [!tldr] Definition
> In a [[Directed graph|digraph]] $G$, the **out-degree** of a vertex $v$ is the number of edges for which $v$ is the head. The **in-degree** of a vertex $v$ is the number of edges for which $v$ is the tail. We use $d_G^+(v)$ to denote the out-degree and $d_G^-(v)$ to denote the in-degree. 

Notes: 
- If $v$ is the head and tail of a loop, then the loop contributes 1 to both the in- and out-degrees of $v$. 

## Examples and Non-Examples

Consider the digraph below: 
![[digraph-example.png|400]]
The in- and out-degrees are as follows: 

| $v$ | In-degree $d_G^-(v)$ | Out-degree $d_G^+(v)$ |
| :-: | -------------------- | --------------------- |
|  1  | 1                    | 1                     |
|  2  | 0                    | 3                     |
|  3  | 3                    | 0                     |
|  4  | 0                    | 1                     |
|  5  | 1                    | 0                     |
## Resources 

 ![](https://www.youtube.com/watch?v=mXoiHgH4mEE)