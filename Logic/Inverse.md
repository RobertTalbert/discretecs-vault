---
aliases: [inverse, inverses]
--- 

#logic

## Definition 

> [!tldr] Definition
> The **inverse** of the [[Conditional statements|conditional statement]] $P \rightarrow Q$ is the conditional statement $(\neg P) \rightarrow (\neg Q)$. That is, we form the inverse by replacing the [[Conditional statements|hypothesis]] and [[Conditional statements|conclusion]] with their [[Negation|negations]]. 

Notes: 

> [!important] **The inverse of a conditional statement is not always  [[logically equivalent]] to the original statement**. 
> 

To see this, here are the [[Truth tables|truth tables]] for $P \rightarrow Q$ and its inverse $(\neg P) \rightarrow (\neg Q)$ side by side (with intermediate columns for the negations): 

| $P$   | $Q$   | $\stackrel{\Downarrow}{P \rightarrow Q}$ | $(\neg P)$ | $(\neg Q)$ | $\stackrel{\Downarrow}{(\neg P) \rightarrow (\neg Q)}$ |
| ----- | ----- | ----------------- | ----------------- | ------- | ------ | 
| True  | True  | True              | False              | False | True | 
| True  | False | False             | False          | True | True
| False | True  | True              | True         | False | False
| False | False | True              | True                  | True | True 

The truth values in rows 2 and 3 are different. For a more real-life example, the statement "If $x > 0$ then $x^2 > 0$" (where $x$ is a real number) is true, but its converse "If $x \leq 0$ then $x^2 \leq  0$" is not true because of the [[counterexample]] $x = -1$ (which is negative, but its square is not). 

## Examples

Here are some conditional statements and their inverses: 

| Statement                        | Converse                         |
| -------------------------------- | -------------------------------- |
| If it's snowing, then it's cold. | If it's not snowing cold, then it's not cold. |
| If $x > 4$ then $x^2 > 16$.      | If $x \leq 4$ then $x^2 \leq 16$.      |
| My coffee being hot is a consequence of it being freshly brewed. | My coffee not being freshly brewed is a consequence of it not being hot. |                                  |                                  |

## Resources 

<iframe src="https://player.vimeo.com/video/588861844?h=3596e8dbfd" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/588861844">Screencast 2.4: Converse, contrapositive, and inverse</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Tutorial: [Converse, inverse, contrapositive](https://www.varsitytutors.com/hotmath/hotmath_help/topics/converse-inverse-contrapositive)
- Video: [Converse, inverse, contrapositive](https://www.mometrix.com/academy/converse-inverse-and-contrapositive/)
