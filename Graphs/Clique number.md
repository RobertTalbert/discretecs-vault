---
aliases:
  - clique
  - Clique
  - clique number
tags:
  - graphs
created: 2024-09-23
updated:
---
---
## Definition 

> [!tldr] Definition
> A **clique** in a [[Graph|graph]] is a set of vertices which are all pairwise adjacent; that is, it is a subgraph of the graph that is a copy of the [[Complete graph|complete graph]] $K_n$. The **clique number** of a graph is the largest $n$ for which there is a clique of size $n$ in the graph. 

Notes: 
* "Clique" is pronounced "CLEEK". 
* The common use of the term "clique" refers to a subgroup of people within a large group, and everyone in the subgroup knows everyone else in the subgroup. That is the same sense as what's meant in a graph. 
* A clique of size $n$ is just a triangle. So, any graph that contains a triangle has a clique number at least (if not bigger than) $3$. 
* It can be proven that the [[Chromatic number|chromatic number]] of a graph must be greater than or equal to its clique number. 

## Examples

The graph below has a clique of size 4 (consisting of of vertices 1, 6, 3, and 4) and several cliques of size 3 (for example, vertices 1, 3, and 4). 
![[clique4.png]]
This graph does not have a clique of size 5, because in such a clique, each of the five vertices in the clique would have to have a degree at least 4 (since each vertex in the clique would be adjacent to all the other vertices in the clique and possibly others outside the clique). But, this graph has just three vertices of degree 4. Similarly there are no cliques of size 6, 7, 8, etc. Therefore the largest clique present has size 4, hence the graph's clique number is 4. 


## Resources 

(video)

Other resources: 
- 

## Practice 
