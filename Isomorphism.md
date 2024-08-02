---
aliases:
  - isomorphism
  - isomorphic
  - Isomorphic
tags:
  - graphs
created: 2024-08-02
updated:
---
---
## Definition 

> [!tldr] Definition
> Two graphs $G_1 = (V_1, E_1)$ and $G_2 = (V_2, E_2)$ are **isomorphic** if there is a [[Bijective|bijection]] $f: V_1 \rightarrow V_2$ (which we call an **isomorphism**) that preserves the edges exactly in both directions. In other words, $\{u,v\}$ is an edge in $G_1$ if and only if $\{f(u), f(v)\}$ is an edge in $G_2$. 

**Notes**: 
- The practical impact of two graphs being isomorphic, is that they might be represented in ways that appear different, but all the essential structures are the same in both. 
- To prove that two graphs are isomorphic requires setting up a function between the vertex sets that is (1) a [[Bijective|bijection]] (that is, both [[Injective|injective]] and [[Surjective|surjective]]) and (2) edge-preserving. 
- Proving that two graphs are *not* isomorphic involves showing that *no such bijection exists*. This is commonly done through [[Indirect proof|proof by contradiction]] or by demonstrating that one graph has a property that is [[Isomorphism invariant|isomorphism invariant]] but the other graph does not have this property. 
- To prove two graphs are not isomorphic, it is not enough to set up a function between the vertex sets that fails to be a bijection, or fails to preserve edges. This can be done even with graphs that are isomorphic. 

## Examples and Non-Examples

The following two graphs are isomorphic: 
![[isomorphism-example.png]]
([Source](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.researchgate.net%2Ffigure%2FIsomorphic-graphs_fig1_275769739&psig=AOvVaw1meLN4vGX82Va777dmGwfI&ust=1722703525920000&source=images&cd=vfe&opi=89978449&ved=0CBQQjhxqFwoTCKiRlfTg1ocDFQAAAAAdAAAAABAJ))
The isomorphism that makes the graphs isomorphic, is the following function $f$ from the vertex set $\{v1,v2,v3,v4,v5\}$ to the other vertex set $\{u1, u2,u3,u4,u5\}$:

|  $v$   | $v1$ | $v2$ | $v3$ | $v4$ | $v5$ |
| :----: | ---- | ---- | ---- | ---- | ---- |
| $f(v)$ | $u1$ | $u2$ | $u3$ | $u4$ | $u5$ |
This function is a bijection because it is [[Injective|injective]] (there are no "collisions") and [[Surjective|surjective]] (every vertex in the [[Codomain|codomain]] is "hit" by at least one vertex in the [[Domain|domain]]). Let's check to see if edges are preserved. For each edge $\{a,b\}$ we will apply the function to the endpoints to get $\{f(a), f(b)\}$ and then see if the result is truly an edge in $H$. 

|             Edge in $G$             | $\{v1, v2\}$ | $\{v1,v3\}$ | $\{v1,v4\}$ | $\{v1,v5\}$ | $\{v2,v3\}$ | $\{v3,v4\}$ | $\{v4,v5\}$ | $\{v5,v2\}$ |
| :---------------------------------: | ------------ | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| After applying $f$ to the endpoints | $\{u1, u2\}$ | $\{u1,u3\}$ | $\{u1,u4\}$ | $\{u1,u5\}$ | $\{u2,u3\}$ | $\{u3,u4\}$ | $\{u4,u5\}$ | $\{u5,u2\}$ |
|        Is it an edge in $H$?        | Yes          | Yes         | Yes         | Yes         | Yes         | Yes         | Yes         | Yes         |
If two graphs are isomorphic, there can be more than one isomorphism between them. For example here is another bijection $g$ on the vertex sets that is also an isomorphism: 

|  $v$   | $v1$ | $v2$ | $v3$ | $v4$ | $v5$ |
| :----: | ---- | ---- | ---- | ---- | ---- |
| $g(v)$ | $u1$ | $u5$ | $u4$ | $u3$ | $u2$ |
Checking that this function preserves edges: 

|             Edge in $G$             | $\{v1, v2\}$ | $\{v1,v3\}$ | $\{v1,v4\}$ | $\{v1,v5\}$ | $\{v2,v3\}$ | $\{v3,v4\}$ | $\{v4,v5\}$ | $\{v5,v2\}$ |
| :---------------------------------: | ------------ | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| After applying $f$ to the endpoints | $\{u1, u5\}$ | $\{u1,u4\}$ | $\{u1,u3\}$ | $\{u1,u2\}$ | $\{u5,u4\}$ | $\{u4,u3\}$ | $\{u3,u2\}$ | $\{u2,u5\}$ |
|        Is it an edge in $H$?        | Yes          | Yes         | Yes         | Yes         | Yes         | Yes         | Yes         | Yes         |

By contrast, here is a function $h$  between the same two vertex sets, that is a bijection but which does **not** preserve edges: 

|  $v$   | $v1$ | $v2$ | $v3$ | $v4$ | $v5$ |
| :----: | ---- | ---- | ---- | ---- | ---- |
| $g(v)$ | $u2$ | $u3$ | $u4$ | $u5$ | $u1$ |
This again is a bijection, but it does not preserve edges because although $\{v1, v3\}$ is an edge in $G$, the edge $\{f(v1), f(v3)\}$ is $\{u2, u4\}$ but this is not an edge in $H$. 

**Non-examples:**

- A graph that has $3$ vertices is not isomorphic to a graph that has $4$ vertices, because no bijection is possible between a [[Set|set]] with [[Cardinality|cardinality]] 3 and one with cardinality 4. In general, graphs that have different numbers of vertices are not isomorphic. The number of vertices in a graph is therefore [[Isomorphism invariant]]. 
- Likewise, two graphs with different numbers of edges are not isomorphic due to the "if and only if" ([[Biconditional statement|biconditional statement]]) about edges in the definition. 
- However, having the same number of vertices and the same number of edges is insufficient 


## Resources 

(video)

Other resources: 
- 

## Practice 
