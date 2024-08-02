---
aliases:
  - connected
  - Connected
  - component
  - Component
  - components
  - Components
tags:
  - graphs
created: 2024-08-02
updated:
---
---
## Definition 

> [!tldr] Definition
> A [[graph]] $G$ is **connected** if, for every pair of distinct [[Graph|vertices]] $u$ and $v$, there is a [[Paths|walk]] or a [[Paths|path]] from $u$ to $v$. Otherwise we say that $G$ is **disconnected**. A **component** of a graph is a maximal connected [[Subgraph|subgraph]]. 

**Notes**: 
- Another way of saying a graph is "disconnected" is that there exist at least two distinct vertices with no walk or path from one to the other. 
- Another way of saying "component" is that a component is a connected piece of a graph that is as large as possible while still being connected. 
## Examples and Non-Examples

In this picture, the red graph on the left is connected but the blue one on the right is disconnected: 
![[connected-examples.png]]
The first graph is connected because there is a path between each pair of distinct vertices. For example 3, 1, 2 is a path from 3 to 2. The second graph is disconnected because although some pairs of distinct vertices have paths between them, some pairs do not: For example there is no path or walk from vertex 3 to vertex 5. 

In the second graph, there are two components: The subgraph consisting of vertices 0, 1, 2, and 3 and the edges $\{0,1\}, \{0,2\}, \{1,2\},$ and $\{1,3\}$ is one component, and the other is the subgraph consisting of vertices 4 and 5 and the edge $\{4,5\}$. Note that while the subgraph consisting of vertices 0, 1, and 2 and the edges $\{0,1\}, \{0,2\}, \{1,2\}$ is connected, it is not a *maximal* connected subgraph; it is not "as large as possible" since there is a connected subgraph that contains it. 

## Resources 

![](https://www.youtube.com/watch?v=z9cTXaLG1kk)