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

(blurb)

## Examples and Non-Examples

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
