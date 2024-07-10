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

***As a visual diagram or network***. This is one of the most common ways that we think about graphs -- as a visual network of [[Graph|nodes]] (often) connected by [[Graph|edges]]. Visual representations make it simple to understand the properties and behavior of a graph, but they are not very useful when using a computer to analyze a graph, or when the graph contains a very large number of nodes or edges. 

![[degree-example-2.png]]


***As a pair of sets (vertex set + edge set)***. The definition of a [[Graph|graph]] gives a graph as a pair of sets: The first set is the set of vertices, and the second set is the set of edges. For example consider the graph below: 
![[Pasted image 20240701115858.png|400]]
can be represented as the vertex-edge set pair  $G = (\{a,b,c,d\}, \{\{a,c\}, \{a,d\}, \{d,c\}, \{a,b\}\})$. This representation gives all the basic information of the graph without resorting to visuals. However, it is somewhat hard to discern any information about the graph's behavior and structure. 

***As a list of edges***. It is possible to represent a graph just as a list of edges, without specifying the vertices. For example, representing the graph $G$ immediately above as an edge set would give $G = \{\{a,c\}, \{a,d\}, \{d,c\}, \{a,b\}\}$. By specifying the endpoints of the edges, we have implicitly given the list of vertices. Representation as an edge list has at least two advantages: First, it's shorter and more compact. Second, it makes it easy to implement in a computer language; for example we could represent this graph in Python as the list `[[a,c], [a,d], [d,c], [a,b]]` whose elements are two-element lists representing the edges. A significant downside to representing as an edge list, is that if there are disconnected vertices (vertices that do not have any edges [[Adjacent|incident]] with them), those vertices will not appear in the list. 

***As a Python dictionary***. The most common way to represent a graph structure in Python and other languages is by using a [dictionary](https://www.w3schools.com/python/python_dictionaries.asp): The keys of the dictionary are the vertices, and the value associated with each key is a list of vertices that are [[Adjacent|adjacent]] to the key. For example, the graph $G$ above that has four vertices would be represented as: 

```python
{a: [b,c,d], b: [a], c: [a,d], d: [a,c]}
```
The larger graph that appears as the first example above would be: 

```python
{1: [3,4,5,6,7], 2: [3,6], 3: [1,2,7], 4: [1,5,7,8], 5: [1,4,7,8], 
 6: [1,7,2], 7: []}
```

As a list of adjacencies. 
As an adjacency matrix. 

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 
