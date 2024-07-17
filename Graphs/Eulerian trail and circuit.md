---
aliases:
  - Euler trail
  - Euler circuit
  - Eulerian
  - Eulerian circuit
tags:
  - graphs
created: 2024-07-17
updated:
---
---
## Definition 

> [!tldr] Definition
> Given a [[Graph|graph]] $G$, we say that $G$ has (or contains) an **Eulerian trail** if there is a [[Paths|trail]] that contains all the [[Graph|edges]] of $G$. We say $G$ has (or contains) an **Eulerian circuit** if there is a [[Paths|circuit]] that contains all the edges of $G$. We also say that $G$ is **Eulerian** if $G$ has an Eulerian circuit. 

**Notes**: 
- Reminders: 
	- A **[[Paths|walk]]** is a nonempty, alternating sequence of [[Graph|vertices]] and edges that starts and ends with a vertex, and in which every [[Graph|edge]] in the sequence is preceded and succeeded by its endpoints.
	- A **[[Paths|trail]]** is a walk with no repeated edge.
	- A **[[Paths|circuit]]** is a trail that starts and ends at the same vertex. 
- Since a circuit is a special kind of trail, an Eulerian circuit is also an Eulerian trail. But not vice versa, since a trail can start and end at different vertices. 
- A graph has an Eulerian trail if and only if there are at most two vertices that have odd [[Degree|degree]]. 
- A graph has an Eulerian circuit (e.g., "is Eulerian") if and only if it has *no* vertices of odd degree -- that is, the degree of every vertex is even. 
- The word "Euler" is pronounced "OIL-er", and "Eulerian" is pronounced "oy-LAYER-ee-an". The concept is named after mathematician [Leonhard Euler](https://en.wikipedia.org/wiki/Leonhard_Euler).

## Examples and Non-Examples

Consider this graph $G$: 
![[degree-graph-example.png]]
This graph $G$ has an Eulerian trail: **4,3,1,2,3,5,2,6,5**. However, it does not have an Eulerian circuit because it has vertices of odd degree ($\deg(4) = 1$ and $\deg(5) = 3$). Any circuit that contains all edges would have to traverse the edge $\{3,4\}$ twice. 

The [[Complete graph|complete graph]] $K_3$ clearly has an Eulerian cycle, namely **1,2,3,1**. As noted, this is also an Eulerian trail. 
![[k3.png|300]]

So does $K_5$, namely **1,5,4,3,5,2,4,1,3,2,1**. 
![[k5.png|300]]

However $K_4$ has neither an Eulerian trail nor an Eulerian cycle because all four of its vertices have degree 3: 
![[k4.png|300]]



## Resources 

![](https://www.youtube.com/watch?v=5M-m62qTR-s)

