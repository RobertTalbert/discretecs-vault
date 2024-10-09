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
> **Dijsktra's Algorithm** is a process for finding the shortest [[Paths|path]] between two [[Graph|vertices]] in a [[Weighted graph|weighted graph]]. In fact, the algorithm produces as "shortest path [[Tree|tree]]" that consists of shortest paths from a source to all other vertices in the graph. 
> 
> The algorithm proceeds as follows: 
> 1. Select a vertex to be the "source", i.e. the starting point of the paths. 
> 2. Create an empty list `VISITED` that will keep track of vertices that are included in the shortest path tree. 
> 3. Assign a distance value to all vertices in the graph. The distance from the source to itself is 0. For all other vertices, initialize the distances as $\infty$ (infinity). 
> 4. While `VISITED` does not contain all the vertices in the graph: 
> 	- Pick a vertex that is not in `VISITED` that has minimum distance value. Call that vertex $u$. 
> 	- Add $u$ to `VISITED`. 
> 	- Update the distance values of all the vertices adjacent to $u$: For each vertex $v$ that is adjacent to $u$, if the total distance from the source to $v$ is less than its current distance value, replace the distance with the new smaller value. Otherwise leave it alone. 
> 
> The algorithm terminates when all vertices in the graph have been added to the `VISTED`


> 
> 1. Select a vertex $v$ in the graph as the starting point. Initialize a list containing the distance of each vertex in the graph to $v$ (where the distance is the total weight of the shortest path between the vertices); initialize all distances to $\infty$ (infinity). 
> 2. Mark all vertices as "unvisited" and create a second list containing all the unvisited vertices. 
> 3. From the list of unvisited vertices, select the current vertex to be the one with the smallest finite distance. 


Notes: 
- In fact, Dijkstra's algorithm produces a [[Tree|tree]] that contains the shortest path starting from a given vertex to *all* other vertices in the graph. 

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 
