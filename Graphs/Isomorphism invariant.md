---
aliases:
  - invariant
  - Invariant
  - isomorphism invariant
tags:
  - graphs
created: 2024-08-02
updated:
---
---
## Definition 

> [!tldr] Definition
> A property of a [[graph]] $G$ is said to be **isomorphism invariant** (or "an" isomorphism invariant) if for any other graph $H$ that is [[Isomorphism|isomorphic]] to $G$, $H$ also has that property. 

Notes: 
- In other words, an isomorphism invariant property "X" is one that satisfies this [[Conditional statements|conditional statement]]: If $G$ has property "X" and $G$ is [[Isomorphism|isomorphic]] to $H$, then $H$ has property "X". 
- This statement is [[Logical equivalence|logically equivalent]] to the statement that **if X is an isomorphism invariant, and $G$ has property $X$ but $H$ does not have that property, then $G$ and $H$ are *not* isomorphic**. Therefore a practical use of isomorphism invariants is to prove that two graphs are not isomorphic: If $G$ has a particular invariant property and $H$ does not, then $G$ and $H$ are not isomorphic. 

## Examples and Non-Examples

- The **number of [[Graph|vertices]]** in a graph is isomorphism invariant. If $G$ has $n$ vertices and $G$ is isomorphic to $H$, then $H$ must also have $n$ vertices -- because an [[Isomorphism|isomorphism]] is a [[Bijective|bijection]] between the vertex [[Set|sets]], therefore the vertex sets must have the same [[Cardinality|cardinality]]. 
- The **number of [[Graph|edges]]** in a graph is similarly isomorphism invariant. 
- **Having a vertex of a given [[degree]] is isomorphism invariant**. For example, if $G$ has a vertex of degree 6 and $G$ is isomorphic to $H$, then $H$ must also have a vertex of degree 6. Here is a proof of that assertion: 

> [!NOTE] **Claim**: If $G$ is a graph that has a vertex of degree $n$, and $G$ is isomorphic to $H$, then $H$ also has a vertex of degree $n$. 
> 
> **Proof**: Assume that $G$ has a vertex (label it as $v$) with degree $n$, and that $G$ is isomorphic to $H$. We want to show that $H$ has a vertex of degree $n$. Since $G$ is isomorphic to $H$, by definition, there is a [[Bijective|bijection]] $f$ from the vertex set of $G$ to the vertex set of $H$ that preserves edges. We  claim that $f(v)$ has degree $n$. 
> 
> Since $\deg(v) = n$ by our initial assumptions, it means that there are $n$ edges connected to $v$. Because $f$ is edge-preserving, there are $n$ edges connected to $f(v)$ as well. Hence $\deg(f(v)) = n$. ◼

- Being [[Connected graph|connected]] is an isomorphism invariant. So, if one graph is connected and another is not, then the two graphs are not isomorphic. Here is a proof of that assertion:

Claim: If $G$ is connected and $G$ is isomorphic to $H$, then $H$ is connected. 

Proof: We use a [[Indirect proof|proof by contradiction]] this time. Assume that $G$ is connected, $G$ is isomorphic to $H$, but (for a contradiction) $H$ is not connected. The latter assumption means that there exist two vertices in $H$, call them $u$ and $v$, that have no walk or path between them. 

Since $G$ and $H$ are isomorphic, there is a bijective, edge-preserving function $f$ from the vertex set of $G$ to the vertex set of $H$. Since $f$ is a bijection, it is [[Surjective|surjective]], so there are vertices $a$ and $b$ in $G$ that map onto $u$ and $v$ respectively; that is, $f(a) = u$ and $f(b) = v$; and these are the only such vertices in $G$ since $f$ is also [[Injective|injective]].  Now, since $G$ is connected, there is a [[Paths|walk]] (possibly a [[Paths|path]]) in $G$ that starts at $a$ and ends at $b$. Denote this walk $a, x_1, x_2, x_3, \dots, x_m, b$ as a list of [[Adjacent|adjacent]] vertices. Since $f$ preserves edges, there is an edge in $H$ between $u = f(a)$ and $f(x_1)$; an edge between $f(x_1)$ and $f(x_2)$, and so on until there is an edge between $f(x_m)$ and $f(b) = v$. each of these edges 


## Resources 

(video)

Other resources: 
- 

## Practice 
