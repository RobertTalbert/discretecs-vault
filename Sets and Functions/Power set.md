---
aliases: [power set]
--- 

#sets-functions 

## Definition 

> [!tldr] Definition
> If $A$ is any set, then its **power set**, denoted $\mathcal{P}(A)$, is the set whose elements are the subsets of $A$. 

Notes: 
- $A$ is not a subset of $\mathcal{P}(A)$; but $A$ is an element of $\mathcal{P}(A)$ since $A$ is a subset of itself. 
- The [[Empty set|empty set]] $\emptyset$ is always an element of $\mathcal{P}(A)$ for any set, since $\emptyset \subseteq A$ for all $A$. 
- If $A$ is finite with $n$ elements, then $|\mathcal{P}(A)|$ (the [[Cardinality|cardinality]] of the power set) is $2^n$. This is a basic fact resulting from the way the [[binomial coefficient]] is defined. 

## Examples

- If $A = \{1,2\}$, then $\mathcal{P}(A) = \{\emptyset, \{1\}, \{2\}, \{1,2\} \}$. 
- If $B$ = $\{x,y,z\}$ then $\mathcal{P}(B) = \{\emptyset, \{x\}, \{y\}, \{z\}, \{x,y\}, \{x,z\}, \{y,z\}, \{x,y,z\}\}$. 
- The power set of the empty set $\mathcal{P}(\emptyset)$ is $\{ \emptyset \}$. That is, $\mathcal{P}(\emptyset)$ is not empty, but contains one element -- namely the empty set itself. 
- The power set of an infinite set is difficult to write in [[Roster notation|roster notation]], so usually we don't. Instead it is merely understood that the power set contains all possible subsets of the base set. For example $\{1,2,3\} \in \mathcal{P}(\mathbb{Z})$. 

## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/606573917?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 3.5: Power set and cardinality"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

Other resources: 
- Tutorial: [Power set](https://www.mathsisfun.com/sets/power-set.html)
- Video: [What is a power set?](https://www.youtube.com/watch?v=0XNSBoqG-1s) 