---
aliases: [difference, set difference]
--- 

#sets-functions 
## Definition 

> [!tldr] Definition
> The **difference** between the [[Set|sets]] $A$ and $B$, denoted either $A - B$ or $A \setminus B$, is the set whose [[Set|elements]] are the elements of $A$ which are not in $B$. 
> 
> In [[Set-builder notation|set-builder notation]], $A \setminus B = \{ x \, : \, x \in A \ \text{and} \ x \not \in B\}$. 

A visual representation of $A \setminus B$ is this Venn diagram: 
![[set difference.png]]

**Notes:**

- The order matters in set differences just as it does in subtraction: $A \setminus B$ is not the same set as $B \setminus A$. See the examples below. 

## Examples 

- If $A = \{1,2,3,4\}$ and $B = \{1,3,5,7,9\}$ then $A \setminus B = \{2,4\}$, and $B \setminus A = \{5,7,9\}$.  
- If $A = \{n \in \mathbb{N} \, : \, n \ \text{is a multiple of 3}\}$ and $B =  \{n \in \mathbb{N} \, : \, n \ \text{is a multiple of 2}\}$ then $A \setminus B$ is the set of natural numbers that are multiples of $3$ but not multiples of $2$ (that is, not even): $\{3, 9, 15, 21, \dots\}$. On the other hand $B \setminus A$ is the set of natural numbers that are multiples of $2$ (i.e. even numbers) but which are not multiples of $3$: $\{2, 4, 8, 10, 14, 16, 20, 22, 26, \dots\}$. 

## Resources 

<iframe src="https://player.vimeo.com/video/606600971?h=e256db4c8a" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/606600971">Screencast 3.6: Set operations</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Video: [Sets and set operations](https://www.youtube.com/watch?v=QiOfsWm3peE&list=PL2419488168AE7001&index=64&pp=iAQB)
- Tutorial: [Difference of sets](https://www.cuemath.com/algebra/difference-of-sets/)
