---
aliases:
  - chromatic index
tags:
  - graphs
created: 2024-07-24
updated:
---
---
## Definition 

> [!tldr] Definition
> Given a [[Graph|graph]] $G$, the **chromatic index** of $G$ is the minimum number of colors in any proper [[Edge coloring|edge coloring]] of $G$. We denote the chromatic index of $G$ by $\chi'(G)$. 

Notes:
- $\chi$ is the Greek letter "chi", pronounced "Kie" (rhymes with "pie"). The symbol $'$ next to the $\chi$ is pronounced "prime". 
- The notation for chromatic index is similar to that of the [[Chromatic number|chromatic number]], which is the minimum number of colors in any [[Vertex coloring|vertex coloring]] of $G$. 

## Examples and Non-Examples

For the [[Complete graph|complete graph]] $K_4$, the chromatic index is $\chi'(K_4) = 3$. Here is an [[edge coloring]] with 3 colors that implements this: 
![[k4-edge-color-3.png|400]]
This example proves only that the chromatic index is *at most* 3; by itself it does not rule out an edge coloring with fewer than three colors. However, in fact, an [[Edge coloring|edge coloring]] of $K_4$ with fewer than three colors is impossible, since each vertex has three edges [[Adjacent|incident]] with it, and each edge must receive a different color. Therefore the chromatic index is exactly 3. 

The chromatic index of $C_n$, the [[Cycle graph|cycle graph]] on $n$ vertices, is 2 if $n$ is even because we can just alternate colors as we go around the cycle. If $n$ is odd, there is an extra edge in the cycle and therefore 3 colors are needed. 

## Resources 

(video)

Other resources: 
- 

## Practice 
