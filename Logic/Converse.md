---
aliases: [converse, converses]
--- 

#logic

## Definition 

> [!tldr] Definition
> The **converse** of the [[Conditional statements|conditional statement]] $P \rightarrow Q$ is the conditional statement $Q \rightarrow P$. That is, we form the converse by switching the [[Conditional statements|hypothesis]] and [[Conditional statements|conclusion]] of the original statement and doing nothing else. 

Notes: 

> [!important] **The converse of a conditional statement is not always  [[logically equivalent]] to the original statement**. 
> 

To see this, here are the [[Truth tables|truth tables]] for $P \rightarrow Q$ and its converse $Q \rightarrow P$ side by side: 

| $P$   | $Q$   | $P \rightarrow Q$ | $Q \rightarrow P$ |
| ----- | ----- | ----------------- | ----------------- |
| True  | True  | True              | True              |
| True  | False | False             | **True**          |
| False | True  | True              | **False**         |
| False | False | True              | True                  |

The truth values in rows 2 and 3 are different. Or to take a more real-life example, the conditional statement "If $x > 0$ then $x^2 > 0$" (where $x$ is a real number) is true, but its converse "If $x^2 > 0$ then $x > 0$" is not true because of the [[counterexample]] $x = -1$. 

If it happens that both $P \rightarrow Q$ and $Q \rightarrow P$, then we say "$P$ [[if and only if]] $Q$". 
## Examples

Here are some conditional statements and their converses: 

| Statement                        | Converse                         |
| -------------------------------- | -------------------------------- |
| If it's snowing, then it's cold. | If it's cold, then it's snowing. |
| If $x > 4$ then $x^2 > 16$.      | If $x^2 > 16$ then $x > 4$.      |
| My coffee being hot is a consequence of it being freshly brewed. | My coffee being freshly brewed is a consequence of it being hot. |                                  |                                  |

## Resources 

<iframe src="https://player.vimeo.com/video/588861844?h=3596e8dbfd" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/588861844">Screencast 2.4: Converse, contrapositive, and inverse</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Tutorial: [Logical converse](https://www.mathsisfun.com/definitions/converse-logic-.html)
- Tutoral: [Converse and contrapositive](https://www.cs.odu.edu/~toida/nerzic/content/logic/prop_logic/converse/converse_intro.html)
