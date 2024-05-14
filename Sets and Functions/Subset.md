---
aliases: [subset, subsets]
--- 
#sets-functions
## Definition 

> [!tldr] Definition
> A set $B$ is a **subset** of another set $A$, if every element of $B$ is also an element of $A$. If $B$ is a subset of $A$, this relationship is denoted $B \subseteq A$.  
> 
> If $B \subseteq A$ but $B \neq A$, we say that $B$ is a **proper subset** of $A$ and write $B \subset A$. 

A visual representation of the relationship $B \subseteq A$ is this Venn diagram: 
![[Pasted image 20230718094622.png|200]]
(This is actually showing that $B$ is a *proper* subset of $A$ since the two are not shown as being equal.)

In terms of logical propositions, $B$ is a subset of $A$ if the following [[Conditional statements|conditional statement]] is true: 

> For every $x$, if $x \in B$ then $x \in A$. 
## Examples and Non-Examples

Examples: 
- The [[natural numbers]] are a (proper) subset of the [[integers]]. (That is, $\mathbb{N} \subseteq \mathbb{Z}$.)
- The set $\{0,1,2,3\}$ is a (proper) subset of $\mathbb{N}$. 
- The set $\{0,2,4\}$ is a (proper) subset of the set $\{0,2,4,6,8\}$. 

> [!important] The empty is a subset of every set
> The empty set $\emptyset$ is a subset of every set. To see this, use the [[Conditional statements|conditional statement]] that defines the subset relationship: *For all $x$, if $x \in B$ then $x \in A$.* Let $B$ be the empty set and let $A$ be any set at all. Then the hypothesis of this statement, $x \in \emptyset$, is always false because nothing is "in" the empty set. Therefore the conditional statement is always true.

Non-examples: 
- The set of [[integers]] is not a subset of the set of [[natural numbers]], because there are elements of the integers that don't belong to the natural numbers, such as $-3$. 
- The set $\{1,2,3\}$ is not a subset of $\{2,3,4\}$ because although these sets have elements in common (i.e. the [[intersection]] is not the empty set), the number $1$ is not an element of the set $\{2,3,4\}$. 

## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/606554057?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 3.4: Subsets and set equality"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>


## Practice 
