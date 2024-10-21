---
aliases:
  - Floyd-Warshall
  - Floyd-Warshall algorithm
tags:
  - digraphs-relations
created: 2024-10-21
updated:
---
---
## Definition 

> [!tldr] Definition
> The **Floyd-Warshall algorithm** is a method for computing the adjacency [[Matrix|matrix]] of the [[Transitive closure|transitive closure]] of a [[Directed graph|directed graph]] using the adjacency matrix of the original [[Directed graph|digraph]]. 
> 
> The algorithm takes the adjacency matrix for the digraph as input, and does the following: 
> 1. Make a copy of the matrix, and call it $W$. This matrix consists of `0` and `1` entries; the algorithm will modify some of the `0` entries to become `1`s. Let $n$ be the number of rows/columns of $W$. 
> 2. For $k$ running from $0$ to $n-1$:
> 	a) Let $i$ run from $0$ to $n-1$ and $j$ run from $0$ to $n-1$
> 	b) For each $(i,j)$-pair. if *either* the $(i,j)$-entry of $W$ is `1`, *or* if the $(i,k)$-entry *and* $(k,j)$-entry of $W$ is `1`, then set the $(i,j)$-entry of $W$ to `1`. (This entry might already be `1`.)
> 3. Return the modified $W$. 


**Notes**: 
* This algorithm is sometimes known as just the "Warshall algorithm". 
* Modifications of this algorithm can also be used to find shortest paths in weighted graphs (and digraph), and solve several other common graph problems. 

## Examples 

The "Part 2" video below shows a completed example. Here is another: 

Consider this directed graph:
![[fw-digraph.png|500]]
Its adjacency matrix is 
$$\begin{bmatrix} 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 0 \\ 1 & 1 & 0 & 1 \\ 1 & 1 & 0 & 0 \end{bmatrix}$$
Initialize $W$ to be this matrix. The number of rows and columns is 4. Note, although the vertices are labelled 1 through 4, to stay consistent with the algorithm we will refer to the rows and columns as being numbered 0 through 3. So row 1 corresponds to vertex 2 for example. 

We begin a threefold `for` loop in which $k$, $i$, and $j$ all loop through the values 0, 1, 2, and 3. This results 

## Resources 

Part 1: 
![](https://www.youtube.com/watch?v=hKCqske0rAE)


Part 2: 
![](https://www.youtube.com/watch?v=BTRssTnhZVU)

Pseudocode from the first video: 
```python
def warshall(M):
    n = M.nrows()
    W = M
    for k in range(n):
        for i in range(n):
            for j in range(n):
                W[i,j] = W[i,j] or (W[i,k] and W[k,j])
    return W
```
