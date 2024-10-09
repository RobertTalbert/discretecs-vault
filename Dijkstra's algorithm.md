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
> The algorithm terminates when all vertices in the graph have been added to the `VISTED` list. The vertices in the visited list can be used to find the shortest path from the source to any other point in the graph. 

## Example

(Adapted from [the example at this website](https://www.javatpoint.com/dijkstras-algorithm))

Here is a weighted graph: 
![[dijkstras-algorithm6.png]]
Let's use Dijkstra's Algorithm to find a shortest-path tree with $A$ as the source node. We have selected $A$ as the source node. Initialize `VISITED` as the empty list. The initial distances are: 

| Vertex | Distance from $A$ |
| :----: | :---------------: |
|  $A$   |        $0$        |
|  $B$   |     $\infty$      |
|  $C$   |     $\infty$      |
|  $D$   |     $\infty$      |
|  $E$   |     $\infty$      |
|  $F$   |     $\infty$      |

The `VISITED` list does not contain all the vertices -- in fact, it's empty. So in step 4, we pick a vertex not in `VISITED` that has the minimum distance value. That vertex is $A$, since its distance is 0 and all others are infinite. So, add $A$ to the `VISITED` list. Then update the distances of all vertices adjacent to $A$, which are $B$ and $C$. To update, look at the current distance values for $B$ and $C$ in the table, and if the total distance from the source to those vertices is less than what is in the table, replace the table value with that distance. Here, the current distance value for $B$ is $\infty$ but its total distance from $A$ is $4$. So update its distance to $4$. Likewise update the distance value for $C$ to $5$. The `VISITED` list is now `[0]`, and the distances are:

| Vertex | Distance from $A$ |
| :----: | :---------------: |
|  $A$   |        $0$        |
|  $B$   |        $4$        |
|  $C$   |        $5$        |
|  $D$   |     $\infty$      |
|  $E$   |     $\infty$      |
|  $F$   |     $\infty$      |

## Resources 

(video)

Other resources: 
- [A walkthrough of Dijkstra's algorithm with a Python implementation](https://www.w3schools.com/dsa/dsa_algo_graphs_dijkstra.php) (uses object-oriented programming)

## Practice 
