---
aliases: [symmetric difference]
--- 

#sets-functions 

## Definition 

> [!tldr] Definition
> If $A$ and $B$ are [[Set|sets]], the **symmetric difference** of $A$ and $B$ is the set whose [[Set|elements]] are all the elements that are in either $A$ or $B$, but not in both. In notation, the symmetric difference of $A$ and $B$ is written $A \triangle B$. In [[Set-builder notation|set-builder notation]], 
> $$A \triangle B = \{ x \, : \, x \in A \cup B \ \text{and} \ x \not \in A \cap B\}$$

A visual representation of $A \triangle B$ is this Venn diagram: 
![[symmetric difference.png|300]]
Image credit: https://www.javatpoint.com/symmetric-difference-between-two-sets

**Notes:**
- We can also define $A \triangle B$ as the [[Set difference|set difference]] between the [[Union|union]] of $A$ and $B$, and the [[Intersection|intersection]] of $A$ and $B$: $A \triangle B = (A \cup B) \setminus (A \cap B)$. 
- The symmetric difference is the set-theory equivalent of the [[Exclusive OR|exclusive or]] operation in logic, and sometimes the same notation is used to denote it: $A \oplus B$. 
## Examples 

- If $A = \{1,2,3,4\}$ and $B = \{1,3,5,7,9\}$ then $A \triangle B = \{1,2,4,5,7,9\}$. That is, the symmetric difference is all elements of $A \cup B$ except $3$ since $3$ is in both sets. 
- If $A = \{n \in \mathbb{N} \, : \, n \ \text{is odd and greater than 3}\}$ and $B =  \{n \in \mathbb{N}  \, : \, n \ \text{is even and greater than 3}\}$ then $A \triangle B = \{4,5,6,7,8,\dots\}$, which in this case is the same as $A \cup B$ since $A$ and $B$ are [[Intersection|disjoint]] (because a natural number greater than 3 cannot be odd and even at the same time). 

## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/606600971?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 3.6: Set operations"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

Other resources: 
- Tutorial: [Symmetric difference between two sets](https://www.javatpoint.com/symmetric-difference-between-two-sets)
