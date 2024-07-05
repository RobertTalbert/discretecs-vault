---
aliases:
  - subgraph
tags:
  - graphs
created: 2024-07-05
updated:
---
---
## Definition 

> [!tldr] Definition
> Given two [[Graph|graphs]] $G_1 = (V_1, E_1)$ and $G_2 = (V_2, E_2)$, we say that $G_1$ is a **subgraph** of $G_2$ if there is a copy of $G_1$ contained within $G_2$. More formally: $G_1$ is a subgraph of $G_2$ if $V_1 \subseteq V_2$ and $E_1 \subseteq E_2$. 

(blurb)

## Examples and Non-Examples

Example: Let $G = K_5$, the [[complete graph]] on five vertices labelled $1,2,3,4,5$: 
![[k5.png|300]]

As a vertex set/edge set pair, this graph is  $G = (V,E)$ where $V = \{1,2,3,4,5\}$ (the vertices) and $E = \{\{1,2\}, \{1,3\}, \{1,4\}, \{1,5\}. \{2,3\}, \{2,4\}, \{2,5\}, \{3,4\}, \{3,5\}, \{4,5\}\}$ (the edges). Now consider the graph $G' = (V', E')$ where $V' = \{1,2,3\}$ and $E' = \{\{1,2\}, \{1,3\}, \{2,3\}\}$. Then $G'$ is a subgraph of $G$ since $V' \subseteq V$ and $E' \subseteq E$. Visually, we can see that a copy of $G'$ is contained in $G$: 

![[subgraph.png|400]]





## Resources 

(video)

Other resources: 
- 

## Practice 
