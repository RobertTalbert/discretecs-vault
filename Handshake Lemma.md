---
aliases: 
tags:
  - graphs
created: 2024-08-02
updated:
---
---
## Definition 

> [!tldr] Definition
> If $G = (V,E)$ is a graph, then the sum of the [[Degree|degrees]] of the [[Graph|vertices]] in $G$ is equal to twice the number of [[Graph|edges]] in $G$. That is, 
> $$\sum_{v \in V} \deg(v) = 2 |E|$$
> where $|E|$ is the [[Cardinality|cardinality]] of $E$. 

**Notes**: 
- The Handshake Lemma is a fundamental theoretical result about graphs and is used in numerous other theorems about them. 
- It is also of practical use, making it possible to count edges (which can be hard) by looping through the degrees of the vertices (which is generally easy). 
- Note that the Handshake Lemma implies that the sum of degrees in any graph must be an [[Even and odd integers|even]] number, since it is 2 times the number of edges. 

## Examples and Non-Examples

- Consider $K_n$, the [[Complete graph|complete graph]] on $n$ vertices. This graph has $n$ vertices, and each vertex is [[Adjacent|adjacent]] to all of the others (but not itself) so $\deg(v) = n-1$ for each vertex $v$. Therefore the sum of the degrees is $n(n-1)$. This is twice the number of edges, so we can conclude that the number of edges in $K_n$ is half of this, or $\dfrac{n(n-1)}{2}$. 
- A graph whose [[Degree|degree sequence]] is $6,6,4,4,4,3,3,2$ must have 16 edges: 
$$\sum_{v \in V} \deg(v) = 6+6+4+4+4+3+3+2 = 32$$


## Resources 

(video)

Other resources: 
- 

## Practice 
