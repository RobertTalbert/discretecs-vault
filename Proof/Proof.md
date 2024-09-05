---
aliases: [proof, proofs]
--- 

#logic #proof 

## Definition 

> [!tldr] Definition
> A **proof** is an explanation for why a [[Propositions|proposition]] is always true under the conditions in which it is stated, that is thorough, free of errors, and clearly expressed. 

Notes: 
- While there is almost never a single "right" way to prove a proposition, there are several commonly accepted methods for approaching a proof, including: 
	- [[Direct proof]]
	- [[Proof by contraposition]]
	- [[Indirect proof|Proof by contradiction]]
	- Proof by [[Mathematical induction|mathematical induction]] or [[Strong induction|strong induction]]
	- Combinatorial proof 
	- As well as simply giving thorough explanations for observed phenomena. 
- 

## Examples and Non-Examples

Here is a very simple proposition: 

> [!NOTE] Proposition
> For all integers $n$, if $n$ is even then $n^2$ is even. 

This proposition appears to be true based on the following examples: 

| $n$   | $0$ | $2$ | $4$  | $6$  | $8$ |
| ----- | --- | --- | ---- | ---- | --- |
| $n^2$ | $0$ | $4$ | $16$ | $36$ | $64$    |

This list of examples provides supporting evidence that the proposition is true, because we have five integers that are all even, and their squares are even. 

**However, this list of examples is not a proof** because the proposition says that if $n$ is even then $n^2$ is even, *for all* integers. This list does not represent all integers, only five of them. 


> [!important] IMPORTANT
> A finite list of examples is not a proof for a global statement about an infinite number of things. 

To prove the proposition, we provide a *proof* that explains why the proposition is true for all integers. **There is typically more than one way to prove a proposition.** Often the strategy and outline of the proof is given by the form of the proposition. In this case, the proposition is a [[Conditional statements|conditional statement]]. These are true in all cases except where the [[Conditional statements|hypothesis]] is true and the [[Conditional statements|conclusion]] is false. So an effective argument (known as "direct proof") is to **assume the hypothesis is true, then show that the conclusion must be true**. 

> [!NOTE] Proof
> Assume that $n$ is any even integer. This means that $n$ is two times some other integer, so $n = 2k$ for some integer $k$. We want to show that $n^2$ is even, that is, $n^2$ is two times some integer, $n^2 = 2m$. Now square both sides of this equation: $n^2 = (2k)^2$. The right side is equal to $4k^2$ which is equal to $2(2k^2)$. The number in parentheses, $2k^2$, is an integer because squaring one integer gives another integer. If we let $m = 2k^2$ we now have $n^2 = 2m$ and this is what we wanted to show. 

This is a correct proof because it is free of computational and logical errors, and is clearly communicated -- although it may not seem clear at first because it is quite dense, and asks you (the reader) to follow some logical steps. And the language is a little stiff. 

But this need not be *the only* correct proof. There are as many ways to explain a true statement as there are people doing the explanation. As long as we are giving a clear, correct explanation that explains why the proposition is *always* true (not just sometimes, as in a list of examples) then it's a proof. 

## Resources 

<iframe width="560" height="315" src="https://www.youtube.com/embed/z-TPb8hI58k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Other resources: 
- Tutorial: [Introduction to mathematical arguments](https://math.berkeley.edu/~hutching/teach/proofs.pdf)
