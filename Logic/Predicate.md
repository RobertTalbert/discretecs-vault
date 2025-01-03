---
aliases: [predicate, predicates]
--- 

#logic 

## Definition 

> [!tldr] Definition
> A **predicate** is a [[Propositions|proposition]] without a definite, fixed truth value but instead its truth value depends on the value of one or more variables. Alternatively, a predicate is a [[Function]] that takes in one or more variables as input, and whose outputs are the values `True` or `False`. (That is, its [[Codomain]] is the [[Set]] `{True, False}`.)

Notes: 
- The truth value of a predicate is undetermined until all variables have been given inputs. By assigning values to the inputs we are [[quantifying]] the predicate. 
- Whereas [[Propositions|propositions]] are notated using single letters (for example, $P$) we typically use [[function notation]] for predicates, indicating the variable or variables in parentheses following a letter; for example $P(n)$ or $Q(x,y)$. 
- The [[domain]] of a predicate refers to the set from which the variables are drawn. 

## Examples and Non-Examples

The statement "The [[natural number]] $n$ is a perfect square" is a predicate because it is neither true nor false -- the truth value depends on the value of $n$. Let $P(n)$ represent this predicate. Then $P(4)$ is True because $4$ is a perfect square ($4 = 2^2$) but $P(5)$ is False because $5$ is not a perfect square. 

The statement "There are $2^n$ [[Binary digits and bitstrings|bitstrings]] of length $n$" is a predicate because of the presence of the variable $n$ (assumed to be a [[Natural numbers|natural number]] because it refers to the size of a set). This predicate happens to be True for every natural number $n$ (a fact that we will prove in several different ways during the course). 

We can represent predicates in Python using functions that return only Boolean values. For example the predicate "The integer $n$ is a multiple of 10" (which is True for $n = 0, \pm 10, \pm 20\, \dots$ and False otherwise) can be implemented like this: 
```python
def P(n): 
	return n % 10 == 0
```
(The `%` symbol is the [[Modulus operator|modulus operator]] in Python.)

## Resources 

<iframe src="https://player.vimeo.com/video/598881354?h=33c858ee70" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/598881354">Screencast 2.8: Predicates</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Book section: [Predicate logic](<https://math.libretexts.org/Bookshelves/Combinatorics_and_Discrete_Mathematics/A_Cool_Brisk_Walk_Through_Discrete_Mathematics_(Davies)/08%3A_Logic/8.2%3A_Predicate_logic>)
- Book section: [Introduction to predicate logic](https://www.cs.odu.edu/~toida/nerzic/content/logic/pred_logic/intr_to_pred_logic.html)
