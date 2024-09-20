---
aliases:
  - Hamilton path
  - Hamilton cycle
  - Hamiltonian cycle
  - Hamiltonian
  - Hamilton circuit
tags:
  - graphs
created: 2024-07-17
updated: 2024-09-20
---
---
## Definition 

> [!tldr] Definition
> Given a [[Graph|graph]] $G$, we say that $G$ has (or contains) a **Hamiltonian path** (or **Hamilton path**) if there is a path that contains all the [[Graph|vertices]] of $G$. We say $G$ has (or contains) a **Hamiltonian cycle** (or **Hamilton cycle**) if there is a cycle that contains all the vertices of $G$. We also say $G$ **is Hamiltonian** if it has a Hamilton cycle. 

Notes: 
- Reminders: 
	- A **walk** is a nonempty, alternating sequence of [[Graph|vertices]] and edges that starts and ends with a vertex, and in which every [[Graph|edge]] in the sequence is preceded and succeeded by its endpoints. If the walk starts and ends with the same vertex, it is called a **closed walk**. 
	- A **trail** is a walk with no repeated edge. If the trail starts and ends with the same vertex, it is called a **closed trail** or **circuit**. 
	- A **path** is a trail with no repeated vertex. A path consisting of a single vertex is called a **trivial path**. 
	- A **cycle** is a closed trail that has at least three (3) different vertices in it, and the only repeating vertices are the first and the last. 
- Therefore a Hamilton path is a nonempty, alternating sequence of vertices in no edges are repeated, *and* in which no vertices are repeated, *and* which contains every vertex in the graph. And a Hamilton cycle is a Hamilton path that starts and ends at the same vertex. (The starting and ending vertex is an exception to the rule about no repeated vertices.) We can conclude that a Hamiltonian cycle is a cycle in a graph that visits every vertex *exactly* once. 
- Hamiltonian structures are named after Irish mathematician [William Rowan Hamilton](https://en.wikipedia.org/wiki/William_Rowan_Hamilton). 
- Determining whether or not a graph has a Hamilton circuit is a question that can be answered with mathematical propositions, such as [[Dirac's Theorem]] and [[Ore's Theorem]]. These give conditions which, when met, guarantee the existence of a Hamilton circuit. But they do not give information on how to find one. 
- The problem of *finding* a specific Hamilton circuit in a graph, on the other hand, is [NP-complete](https://en.wikipedia.org/wiki/NP-completeness). In layperson's terms this means that while it is computationally easy to *verify* whether a given cycle is Hamiltonian, there is no known way to *find* such a cycle quickly. (Contrast with the similar problem for [[Eulerian trail and circuit|Eulerian circuits]], where there is a simple theorem that will detect the existence of such circuits and the proofs of those theorems consist of algorithms that construct the Euler circuit directly.) 

## Examples and Non-Examples

Consider this graph $G$: 
![[degree-graph-example.png]]
There are multiple Hamiltonian paths in this graph, for example **4,3,1,2,6,5** and **6,5,2,1,3,4**. But there is no Hamiltonian cycle, because any Hamiltonian cycle would have to include vertex 4, and would require visiting vertex 3 twice. 

The [[Cycle graph|cycle graph]] $C_4$ clearly has a Hamiltonian cycle (therefore also a Hamiltonian path), **1,2,3,4,1**. In fact every cycle graph has one by just going around the cycle. 
![[c4.png|300]]

Every [[Complete graph|complete graph]] is also Hamiltonian, because the complete graph $K_n$ contains $C_n$ as a [[Subgraph|subgraph]], and the Hamiltonian cycle can be found by tracing around that subgraph. For example, here is a Hamiltonian cycle in $K_5$ found by tracing $C_5$: 
![[c5-in-k5.png|400]]



## Resources 

![](https://www.youtube.com/watch?v=6QFSkhcHLiA)

![](https://www.youtube.com/watch?v=IADKmt_fXbM)
