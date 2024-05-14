---
aliases: [contrapositive, contrapositives]
--- 

#logic

## Definition 

> [!tldr] Definition
> The **contrapositive** of the [[Conditional statements|conditional statement]] $P \rightarrow Q$ is the conditional statement $(\neg Q) \rightarrow (\neg P)$. That is, we form the converse by replacing the [[Conditional statements|hypothesis]] of the original statement with the [[Negation|negation]] of the original conclusion, and replacing the [[Conditional statements|conclusion]] of the original statement the [[negation]] of the original hypothesis. 

Notes: 

> [!important] **The contrapositive of a conditional statement is always  [[logically equivalent]] to the original statement**. 
> 

To see this, here are the [[Truth tables|truth tables]] for $P \rightarrow Q$ and its contrapositive $(\neg Q) \rightarrow (\neg P)$ side by side (with intermediate columns for the negations): 

| $P$   | $Q$   | $\stackrel{\Downarrow}{P \rightarrow Q}$ | $(\neg Q)$ | $(\neg P)$ | $\stackrel{\Downarrow}{(\neg Q) \rightarrow (\neg P)}$ |
| ----- | ----- | ----------------- | ----------------- | ------- | ------ | 
| True  | True  | True              | False              | False | True | 
| True  | False | False             | True          | False | False
| False | True  | True              | False         | True | True
| False | False | True              | True                  | True | True 

The original statement is in column 3 and the contrapositive in column 6 (indicated by vertical arrows). Notice the truth values are the same. 

## Examples

Here are some conditional statements and their contrapositives: 

| Statement                        | Converse                         |
| -------------------------------- | -------------------------------- |
| If it's snowing, then it's cold. | If it's not cold, then it's not snowing. |
| If $x > 4$ then $x^2 > 16$.      | If $x^2 \leq  16$ then $x \leq  4$.      |
| My coffee being hot is a consequence of it being freshly brewed. | My coffee not being freshly brewed is a consequence of it not being hot. |                                  |                                  |

## Resources 

<iframe src="https://player.vimeo.com/video/588861844?h=3596e8dbfd" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/588861844">Screencast 2.4: Converse, contrapositive, and inverse</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Tutorial: [Contrapositive](https://www.regentsprep.org/contrapositive/)
- Tutoral: [Converse and contrapositive](https://www.cs.odu.edu/~toida/nerzic/content/logic/prop_logic/converse/converse_intro.html)
