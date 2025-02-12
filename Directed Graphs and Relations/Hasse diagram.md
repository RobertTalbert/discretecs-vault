---
aliases: 
tags:
  - digraphs-relations
created: 2024-11-03
updated:
---
---
## Definition 

> [!tldr] Definition
> Let $X$ be a [[Partial ordering|partially ordered set]] with [[Partial ordering|partial ordering]] $\sim$. The **Hasse diagram** for $X$ is a visual diagram similar to a [[Directed graph|directed graph]] but made with slightly different rules: 
> 
> 1. Draw a vertex for each element of $X$, but arrange them visually so that if $a \sim b$ in the [[Partial ordering|poset]], the vertex for $a$ appears lower in the drawing than the vertex for $b$. 
> 2. The vertices for $a$ and $b$ are joined by a line segment (not an arrow) if $a \sim b$ and if there is no $c$ with $a \sim c$ and $c \sim b$. That is, we ignore "transitive edges".  
> 3. Do not draw any self-loops. 


**Notes**: 
- The Hasse diagram for a poset captures all the information that a [[Directed graph|digraph]] would, but it uses the visual "vertical" arrangement of vertices to imply the direction of arrows,  and uses the [[Reflexive property|reflexive]] and [[Transitive property|transitive]] properties of the partial ordering to remove edges from the picture. 

## Examples 

* Let $X = \{1, 2, 3, 4, 6, 12\}$ with the [[Divisibility|divides]] partial ordering (that is, $a \sim b$ if and only if $a$ divides $b$). The ordinary directed graph for this relation looks like this: 

![[hass-diagram-1.png|500]]
*Note: The code for generating this directed graph is given below.* 

The Hasse diagram would 
* Remove all the self-loops
* Remove any edges that are implied by the transitive property. For example the edge pointing directly from 3 to 12 would not be drawn, because it would be implied by the edge from 3 to 6 and the edge from 6 to 12. 
* Rearrange the vertices so that 1 is at the bottom, 12 is at the top, and the others are arranged by ordering. 

The finished product looks like this: 
![[hasse-diagram-2.png]]
* Let $A = \{a,b,c\}$ and consider the poset $X = {\cal{P}}(A)$ with the $\subseteq$ ordering. The elements of the ground set are the eight subsets of $X$: $\emptyset$, $\{a\}$, $\{b\}$, $\{c\}$, $\{a,b\}$, $\{a,c\}$, $\{b,c\}$, $\{a,b,c\}$. Given two elements $S$ and $T$, $S \sim T$ if $S \subseteq T$. So for example $\{a\} \sim \{a,b\}$ and $\{a,b\} \sim \{a,b,c\}$. Especially note that $\emptyset$ is related to every other element in the set. The Hasse diagram for this poset is: 
![[hasse-diagram-3.png]]
## Resources 

![](https://www.youtube.com/watch?v=i8XeVATqeag)

![](https://www.youtube.com/watch?v=ITv_74xUBdk)


**Code for generating the directed graph above in Python:**

```python
# Python/networkX code for generating the directed graph above

import networkx as nx
import matplotlib.pyplot as plt

p = [(a,b) for a in [1,2,3,4,6,12] for b in [1,2,3,4,6,12] if b % a == 0]
G = nx.DiGraph()
G.add_edges_from(p)

pos = nx.circular_layout(G)
nx.draw(G, pos, node_color='lightgray', with_labels=True)
```