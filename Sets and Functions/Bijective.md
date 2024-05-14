---
aliases: [bijective, bijection]
--- 

#sets-functions 

## Definition 

> [!tldr] Definition
> A [[Function|function]] $f: A \rightarrow B$ is **bijective** if it is both [[Injective|injective]] and [[Surjective|surjective]]. 

**Notes:**
- If a function is bijective it informally means two things: 
	- There are no "collisions" (because the function is injective)
	- There are no points in the codomain that are "left out" (because the function is surjective)
- If there is a bijection between $A$ and $B$, then those two [[Set|sets]] have the same [[Cardinality|cardinality]]. The [[Converse|converse]] is also true for finite sets: If $A$ and $B$ are finite and have the same number of elements, then it's possible to create a bijection between them.

## Examples and Non-Examples

- The function $f: A \rightarrow B$ shown in the diagram below is a bijection:

![[injective1.png|300]]
([Image source](https://www.google.com/url?sa=i&url=https%3A%2F%2Fcollegedunia.com%2Fexams%2Fbijective-function-mathematics-articleid-5395&psig=AOvVaw3bIRWsNf8Mn9zace0S4B8A&ust=1696082301870000&source=images&cd=vfe&opi=89978449&ved=0CBIQjhxqFwoTCLj4zor9z4EDFQAAAAAdAAAAABAE))

- The function $g: \mathbb{Z} \rightarrow \mathbb{Z}$ given by the formula $g(n) = n + 1$ is a bijection. 
- Let $A$ be the set of all $8$-bit strings that have exactly two `1` bits (for example `10100000`) and $B$ the set of all $8$-bit strings that have exactly six `1` bits (like `00111111`). Then the function $f: A \rightarrow B$ that flips all `0` bits in the input to `1`s and vice versa, is a bijection. (Therefore there are exactly the same number of 8-bit strings with 2 `1` bits, as there are 8-bit strings with 6 `1` bits.)
- Let $S$ be any finite set with $n$ elements, written as $S = \{a_1, a_2, a_3, \dots, a_n\}$. If $A \in \cal{P}(S)$ (meaning that $A$ is a subset of $S$) then let $f(A)$ be the $n$-bit string defined as follows: For each $i$ from $1$ to $n$, set the $i$th bit of the string equal to $0$ if $a_i \not \in A$ and set it equal to $1$ if $a_i \in A$. (For example if $S = \{a_1, a_2, a_3, a_4\}$ then $f(\{a_2, a_3\})$ is `0110`.) This function is a bijection, and it tells us that the number of subsets of $S$ is exactly the same as the number of $n$-bit strings if $S$ has $n$ elements. 

Here are some non-examples: 
- The function shown below is not a bijection because it is not injective (although it is surjective): 
![[surj-not-inj.png|150]]
- The function $g: \mathbb{Z} \rightarrow \mathbb{Z}$ given by the formula $g(n) = 2n + 1$ is *not* a bijection because the function is not [[surjective]]: There is no integer in the [[domain]] that maps onto the number $2$, for example. (That number would have to be $n=1/2$ but this is not in the domain.) 



> [!danger] A bijection between sets does not always mean the sets have the same number of elements
> For *finite* sets, if there is a bijection between the sets, then the sets have "the same number of elements". But if the sets are *infinite*, this need not be the case. 
> 
> Consider this example: Let $f: \mathbb{N} \rightarrow \mathbb{Z}$ be the function defined by the following rules:
> 1. If $n$ is odd, then $f(n) = n$. 
> 2. If $n$ is even, then $f(n) = -n/2$. 
>    
> So $f(0) = 0, f(1) = 1, f(2) = -1, f(3) = 3, f(4) = -3$, and so on. This mapping is a bijective function because the function is injective (no two inputs map to the same output) and because the function is surjective (given $y \in \mathbb{Z}$, if $y$ is positive then $y \in \mathbb{N}$ maps onto it; if $y$ is negative then $-2y \in \mathbb{N}$ maps onto it). 
> 
> However clearly $\mathbb{N}$ and $\mathbb{Z}$ do not have "the same number of elements", since $\mathbb{N}$ is a proper [[subset]] of $\mathbb{Z}$. 
> 
> The notion of "the number of elements" in a set breaks down if the sets are infinite. 
 


## Resources 
<iframe src="https://player.vimeo.com/video/614541763?h=7c14d8d686" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/614541763">Screencast 3.11: Bijective functions</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

- Tutorial: [Bijective functions](https://byjus.com/maths/bijective-function)