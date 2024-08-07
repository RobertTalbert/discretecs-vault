---
aliases:
  - relation
tags:
  - digraphs-relations
created: 2024-08-07
updated:
---
---
## Definition 

> [!tldr] Definition
> Given a nonempty [[Set|set]] $X$, a **binary relation** (or just a **relation**) **on $X$** is a [[subset]] of the [[Cartesian product]] $X \times X$. That is, a relation on $X$ is any [[set]] of ordered pairs $(x_1,x_2)$ with $x_1, x_2 \in X$. 

Notes: 
- The [[set]] $X$ is referred to as the *ground set*. 
- If $R$ is a relation on $X$, it means $R \subseteq X \times X$. If $(a,b) \in R$, we sometimes write this as $aRb$ and say "$a$ is related to $b$". 
- Since relations consist of ordered pairs of the ground set $X$, **every finite relation $R$ can be visualized as a [[Directed graph|directed graph]] whose vertex set is $X$ and whose edge set is the relation**. 
- Likewise, **every [[Directed graph|digraph]] is a relation** where the ground set is $X$, and $(a,b)$ is an edge if $aRb$ (that is, $(a,b) \in R$). 
- The symbol $\sim$ is often used to denote a relation. 
- Relations are sometimes described verbally, or in terms of mathematical or quantitative relations. See below for examples. This makes it easy at times to write relations using [[Set-builder notation|set-builder notation]]. 
- The empty subset of $X \times X$ is allowed as a relation on $X$. 

## Examples 

- The set $\{(1,2), (1,3), (2,4)\}$ is a relation on the set $\{1,2,3,4\}$. 
- Define a relation $\sim$ on the set $X = \{1,2,3,4,5,6\}$ using the following rule: $a \sim b$ [[Biconditional statement|if and only if]] $a$ [[Divisibility|divides]] $b$ (that is, $b$ is a multiple of $a$). Then the relation is the following set: 
$$\{(1,2), (1,3), (1,4), (1,5), (1,6), (2,4), (2,6), (3,6), (1,1), (2,2), (3,3), (4,4), (5,5), (6,6)\}$$
- Define another relation, also called $\sim$, on the set $X = \{1,2,3,4,5,6\}$ by declaring $a \sim b$ [[Biconditional statement|if and only if]] $b \, \% \, a = 2$ (where `%` is the [[The modulus operator|modulus operator]]). Then the relation is the following set: 
$$\{(3, 2), (4, 2), (5, 2), (6, 2), (3, 5), (4, 6) \}$$
- The following [[Directed graph|digraph]] visually represents the relation from the previous point: 
![[relation-digraph.png|400]]
- Relations can be put on any set of objects. For example consider $X$ to be the set of words `{cat, bat, cup, cake, bake, shake}`. Let $R$ be the relation on $X$ where if $w$ and $v$ are words in $X$, then $wRv$ if and only if $w$ and $v$ are different words and $w$ rhymes with $v$. Then $R$ is the set `{(cat, bat), (bat, cat), (cake, bake), (cake, shake), (bake, cake), (shake, cake), (bake, shake), (shake, bake)}`. (Note, there are no duplicates in this set: `(cat, bat)` and `(bat, cat)` are different pairs; we cannot assume that if one pair is in the relation then its reverse is also in the relation.) 
- Social networks can be modeled using relations. For example if $X$ is the set of all [LinkedIn](https://www.linkedin.com/) users, then given two users $a$ and $b$, we can say $a \sim b$ if $a$ and $b$ are "connected" on LinkedIn. See the video below for more on relations and social networks. 


## Resources 

![](https://www.youtube.com/watch?v=qnjxdlpWMLA)
