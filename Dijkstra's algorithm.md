---
aliases: 
tags:
  - graphs
created: 2024-10-07
updated:
---
---
## Definition 

> [!tldr] Definition
> **Dijsktra's Algorithm** is a process for finding the shortest [[Paths|path]] between two [[Graph|vertices]] in a [[Weighted graph|weighted graph]]. 
> 
> 1. Select a vertex $v$ in the graph as the starting point. Initialize a table of distances from $v$ to the other vertices in the graph by setting the initial distance to $\infty$ (infinity). Also initialize a list of vertices that have been "visited" -- in practice, we initialize a list of *unvisited* vertices, containing all the vertices in the graph (including the starting point). 
> 2. Mark the starting point as having been visited (for example, by removing it from the unvisited list). 
> 3. Check the distance from $v$ to its neighbors. Update the distances to those neighbors in the first list (that holds the distances from $v$). 
> 4. Once the distances are updated: Select the vertex that is closest to $v$ based on the current known distances. Mark that vertex as visited, and add it to the path. 

Notes: 
- In fact, Dijkstra's algorithm produces a [[Tree|tree]] that contains the shortest path starting from a given vertex to *all* other vertices in the graph. 

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 