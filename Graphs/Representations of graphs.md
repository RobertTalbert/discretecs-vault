---
aliases:
  - representation
  - graph representation
tags:
  - graphs
created: 2024-07-01
updated: 2024-07-10
---
---
## Definition 

[[Graph|Graphs]] can be **represented** in different ways, each having its own particular use case. Here are some of the most common representations. 

*As a visual diagram or network*. This is one of the most common ways that we think about graphs -- as a visual network of [[Graph|nodes]] (often) connected by [[Graph|edges]]. Visual representations make it simple to understand the properties and behavior of a graph, but they are not very useful when using a computer to analyze a graph, or when the graph contains a very large number of nodes or edges. 

![[degree-example-2.png]]


*As a pair of sets (vertex set + edge set)*. The definition of a [[Graph|graph]] gives a graph as a pair of sets: The first set is the set of vertices, and the second set is the set of edges. For example consider the graph below: 
![[Pasted image 20240701115858.png|400]]
can be represented as the vertex-edge set pair  $G = (\{a,b,c,d\}, \{\{a,c\}, \{a,d\}, \{d,c\}, \{a,b\}\})$. This representation gives all the basic information of the graph without resorting to visuals. However, it is somewhat hard to discern any information about the graph's behavior and structure. 

*As a list of edges*. It is possible to represent a graph just as a list of edges, without specifying the vertices. For example, representing the graph $G$ immediately above as an edge set would give $G = \{\{a,c\}, \{a,d\}, \{d,c\}, \{a,b\}\}$. By specifying the endpoints of the edges, we have implicitly given the list of vertices. Representation as an edge list has at least two advantages: First, it's shorter and more compact. Second,

As a list of adjacencies. 

As a Python dictionary. 

As an adjacency matrix. 

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 
