---
aliases:
  - weighted graph
  - weight
  - weights
tags:
  - graphs
created: 2024-08-15
updated: 2024-10-02
---
---
## Definition 

> [!tldr] Definition
> A **weighted graph** is a [[Graph|graph]] in which every [[Graph|edge]] is assigned a numerical value which we call a **weight**. 

Notes: 
- The weights in a weighted graph can be [[Integers|integer]] or non-integer, positive or negative or zero. 
- A [[Directed graph|directed graph]] can also have weighted edges. 
- In applications, the weight of an edge often represents a "cost". For example, a graph representing a highway map could use cities as the vertices, and the weight of an edge between cities could represent the distance between the cities, or the time needed to get from one city to the other, or the cost of road tolls or airfare between them. 

## Examples

Here is an example of a weighted graph: 
![[weighted.png]]

The weight of edge $\{3,4\}$ is 1. The weight of edge $\{5,6\}$ is 8. 

We can represent a weighted graph by modifying existing ways of [[Representations of graphs|representation]] of an unweighted graph: 

- A weighted graph can be given as an adjacency matrix by replacing the "1" in the entry that represents an edge, with the weight of the edge. 
- A weighted graph can be given in "edge list" form by replacing the list of edges with a dictionary whose keys are the edges and the value of a key is the weight of the edge. 
## Resources 

![](https://www.youtube.com/watch?v=MurOpIGCmhQ)
