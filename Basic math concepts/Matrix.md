---
aliases:
  - matrix
  - Matrices
  - matrices
tags:
  - basic-concepts
created: 2024-10-21
updated:
---
---
## Definition 

> [!tldr] Definition
> A **matrix** is a rectangular array of numbers. The plural of "matrix" is **matrices**. Matrices are composed of **rows** (that run horizontally or left-right) and **columns** (that run vertically or up-down). 
> 
> A matrix with $m$ rows and $n$ columns is called an $m \times n$ ("m by n") matrix. A matrix that has the same number of rows as it has columns is called a **square** matrix. 
> 
> The **$(i,j)$-th entry** of a matrix is the element that is in row $i$, column $j$. 

**Notes:**
- Matrices are usually enclosed in either large brackets, or large parentheses. 
- Matrices are a fundamental way to represent [[Graph|graphs]] and [[Directed graph|digraphs]]. We can do so using adjacency matrices or incidence matrices; see below. 

## Examples 

Here is an example of a $3 \times 2$ matrix: 
$$\begin{bmatrix} 1 & 1 \\ 0 & 2 \\ 1 & 3 \end{bmatrix}$$
This matrix is *not* square. The number $3$ is in row 3, column 2. That is, $3$ is the $(3,2)$ element of this matrix. 

Given an undirected [[Graph|graph]], we can represent it as a matrix by creating a square matrix whose rows and columns are indexed by the [[Graph|vertices]] of the graph, and the $(i,j)$ entry is $1$ is vertex $i$ is [[Adjacent|adjacent]] to vertex $j$ and $0$ otherwise. This is known as the **adjacency matrix** for the graph. For example, given this graph: 
![[small-graph.png|400]]
Its adjacency matrix is: 
$$\begin{bmatrix}
0 & 1 & 1 & 1 & 1 \\
1 & 0 & 1 & 1 & 0 \\
1 & 1 & 0 & 1 & 1 \\
1 & 1 & 1 & 0 & 0 \\
1 & 0 & 1 & 0 & 0 
\end{bmatrix}$$

For a [[Directed graph|directed graph]], the $(i,j)$ entry is $1$ if there is a directed edge from vertex $i$ to vertex $j$, and $0$ otherwise. For example, given this digraph: 
![[small-digraph.png|400]]
Its adjacency matrix is: 
$$\begin{bmatrix}
0 & 0 & 1 & 0 & 1 \\
0 & 0 & 1 & 1 & 0 \\
1 & 0 & 0 & 1 & 1 \\
0 & 0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 
\end{bmatrix}$$

## Resources 

(video)

Other resources: 
- 

## Practice 
