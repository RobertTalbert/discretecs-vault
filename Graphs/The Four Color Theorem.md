---
aliases: 
tags:
  - graphs
created: 2024-07-24
updated:
---
---
## Definition 

> [!tldr] Definition
> The **Four Color Theorem** states that **every [[Planar graph|planar]] graph has a proper coloring with no more than four colors.** In other words, every planar graph is four-colorable. 

Notes: 
- The [[Contrapositive|contrapositive]] of the Four Color Theorem says: *If a graph does not have a 4-coloring (that is, a proper coloring with 4 colors) then the graph is not planar*. This provides one way to determine if a graph is non-planar. 
- However, the [[Converse|converse]] of the Four Color Theorem says: *If a graph has a 4-coloring, then the graph is planar*. This statement is **false**; see the examples below. Therefore the existence of a 4-coloring does not imply anything about planarity. 
- The Four Color Theorem was famously [proven in 1989 using a computer](http://www.ams.org/books/conm/098/), by reducing the problem to a very large but finite number of cases and then exhausting each case by brute force. 

## Examples and Non-Examples

A popular application of the Four Color Theorem is coloring regions on a map. Consider this map of the lower 48 United States: 
![[usa-map-blank.png]]
We can think of this map as a graph, where each state is a vertex and two vertices are [[Adjacent|adjacent]] if they share a linear section of a border (disregard places where states meet at only a point, like Arizona and Colorado). Then clearly this graph would be planar, hence we can color in the states using only four colors, with no two adjacent states having the same color. For example: 
![[usa-map-colored.png]]



More examples/non-examples:
- The complete graph on 6 vertices $K_6$ cannot be colored with fewer than 6 colors, since each vertex is adjacent to the remaining five. Therefore the contrapositive of the Four Color Theorem says $K_6$ is nonplanar. (A fact also concluded using [[Kuratowski's Theorem]].)
- Just because a graph has a 4-coloring, it does not mean the graph is planar. For example $K_{3,3}$ (the complete bipartite graph with 3 vertices in each partition) has a 4-coloring, in fact it has a 2-coloring (below). But $K_{3,3}$ is nonplanar due to [[Kuratowski's Theorem]]. Therefore the [[converse]] of the Four Color Theorem is false. 

![[k33-colored.png|400]]
(You can make this into a proper 4-coloring by changing the colors on any two of the vertices to yellow and green.) 


## Resources 

(video)

Other resources: 
- [Every Planar Map is Four Colorable](http://www.ams.org/books/conm/098/) 

## Practice 
