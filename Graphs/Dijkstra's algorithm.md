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

The `VISITED` list does not contain all the vertices -- in fact, it's empty. So in step 4, we pick a vertex not in `VISITED` that has the minimum distance value. That vertex is $A$, since its distance is 0 and all others are infinite. So, add $A$ to the `VISITED` list. Then update the distances of all vertices adjacent to $A$, which are $B$ and $C$. To update, look at the current distance values for $B$ and $C$ in the table, and if the total distance from the source to those vertices is less than what is in the table, replace the table value with that distance. Here, the current distance value for $B$ is $\infty$ but its total distance from $A$ is $4$. So update its distance to $4$. Likewise update the distance value for $C$ to $5$. The `VISITED` list is now `[A]`, and the distances are:

| Vertex | Distance from $A$ |
| :----: | :---------------: |
|  $A$   |        $0$        |
|  $B$   |        $4$        |
|  $C$   |        $5$        |
|  $D$   |     $\infty$      |
|  $E$   |     $\infty$      |
|  $F$   |     $\infty$      |
The `VISITED` list does not contain all the vertices, so we repeat step 4: Pick a vertex that is not in `VISITED` that has minimum distance. This time that vertex is $B$. Add this to `VISITED`. Now update the total distances of all vertices adjacent to $B$: 

- $A$ is adjacent to $B$, and its current distance is $0$. This will never be updated because no distance will be less than $0$. So leave the distance from $A$ alone. 
- $C$ is adjacent to $B$ and its current distance value is $5$. The total distance from $A$ going through $B$, is 15. This is greater than $5$, so **leave the distance value alone**. 
- $D$ is adjacent to $B$ and its current distance is infinite. The total distance from $A$ going through $B$ is 13. This is less than $\infty$ so **update the distance to $D$, to $13$. 
- Likewise, update the distance to $E$, to $11$. 

`VISITED` is now `[A,B]` and the distance list is: 

| Vertex | Distance from $A$ |
| :----: | :---------------: |
|  $A$   |        $0$        |
|  $B$   |        $4$        |
|  $C$   |        $5$        |
|  $D$   |       $13$        |
|  $E$   |       $11$        |
|  $F$   |     $\infty$      |
The `VISITED` list does not contain all the vertices, so we repeat step 4: Pick a vertex that is not in `VISITED` that has minimum distance. This time that vertex is $C$. Add this to `VISITED`.  Now update the total distances of all vertices adjacent to $C$: 

- $A$ is adjacent to $C$, and its current distance is $0$. This will never be updated because no distance will be less than $0$. So leave the distance from $A$ alone. 
- $B$ is adjacent to $C$ and its current distance is $4$. The total distance to $B$ going through $C$ is 16, so do not update $B$'s distance. 
- $E$ is adjacent to $C$ and its current distance is $11$ (this uses the path $A, B, E$). The distance to $E$ going through $C$ on the other hand is $8$. So update the distance for $E$ to $8$. 

`VISITED` is now `[A,B,C]` and the distance list is: 

| Vertex | Distance from $A$ |
| :----: | :---------------: |
|  $A$   |        $0$        |
|  $B$   |        $4$        |
|  $C$   |        $5$        |
|  $D$   |     $13$      |
|  $E$   |     $8$      |
|  $F$   |     $\infty$      |
The `VISITED` list does not contain all the vertices, so we repeat step 4: Pick a vertex that is not in `VISITED` that has minimum distance. This time that vertex is $E$. Add this to `VISITED`.  Now update the total distances of all vertices adjacent to $E$: 

- $B$: The current distance is $4$. The distance from $A$ to $B$ going through $E$ is $8+7 =15$, so do not update. 
- $C$: The current distance is $5$. The distance from $A$ to $C$ going through $E$ (we would go from $A$ to $C$, then to $E$, then backtrack to $C$) is $8+3 =11$, so do not update.
- $D$: The current distance is $13$. The distance from $A$ to $D$ going through $E$ is $8+13 =21$, so do not update. 
- $F$: The current distance is $\infty$. The distance from $A$ to $F$ going through $E$ is $8+6 =14$, which is less than the current distance, so update this distance. 

`VISITED` is now `[A,B,C,E]` and the distance list is: 

| Vertex | Distance from $A$ |
| :----: | :---------------: |
|  $A$   |        $0$        |
|  $B$   |        $4$        |
|  $C$   |        $5$        |
|  $D$   |       $13$        |
|  $E$   |        $8$        |
|  $F$   |       $14$        |

The `VISITED` list does not contain all the vertices, so we repeat step 4: Pick a vertex that is not in `VISITED` (at this point these are only $D$ and $F$) that has minimum distance. This time that vertex is $D$. Add this to `VISITED`.  Now update the total distances of all vertices adjacent to $D$: 

- $B$: The current distance is $4$. The distance from $A$ to $B$ going through $D$ is $13+9=22$, so do not update. 
- $E$: The current distance is $8$. The distance from $A$ to $E$ going through $D$ is $13+13 =26$, so do not update.
- $F$: The current distance is $14$. The distance from $A$ to $F$ going through $D$ is $13+2 =15$, so do not update. 

`VISITED` is now `[A,B,C,E,D]` and the table of distances is unchanged. 

The last vertex to be added is `F`. The `VISITED` list now contains all the vertices of the graph, so the algorithm terminates. 

The data from Dijkstra's Algorithm keeps track of which paths to take from $A$ to reach all the other vertices with the shortest total length: 

| Vertex | Path from $A$ of shortest length | Distance |
| :----: | -------------------------------- | -------- |
|  $A$   | $A$                              | $0$      |
|  $B$   | $A,B$                            | $4$      |
|  $C$   | $A, C$                           | $5$      |
|  $D$   | $A,B,D$                          | $13$     |
|  $E$   | $A,C,E$                          | $8$      |
|  $F$   | $A,C,E,F$                        | $14$     |
## Resources 

![](https://www.youtube.com/watch?v=bZkzH5x0SKU)

Other resources: 
- [A walkthrough of Dijkstra's algorithm with a Python implementation](https://www.w3schools.com/dsa/dsa_algo_graphs_dijkstra.php) (uses object-oriented programming)

## Practice 
