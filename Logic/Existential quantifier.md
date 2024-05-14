---
aliases: [existential quantifier, existentially quantified]
--- 

#logic
## Definition 

> [!tldr] Definition
> A [[Predicate|predicate]] is **existentially quantified** when we assert that the predicate is true for one or more values of its variables; that is, when we assert that a value of the input exists that makes the predicate true. An **existential quantifier** is a logical operator that declares that the predicate is true for all values of a variable. If $P(x)$ is a predicate, then the statement "There exists an $x$, such that $P(x)$ is true" is its existentially quantified form. Symbolically we write this as $\exists x P(x)$. 

Notes: 
- Whereas the single-variable predicate $P(x)$ is not a [[Propositions|proposition]] because its truth value depends on the input $x$, its existentially quantified form $\exists x P(x)$ is a proposition with a definite truth value. For example, the statement "The integer $n$ is even" is a predicate that is sometimes true and sometimes false; the quantified form "There exists an integer $n$, such that $n$ is even" is definitely true (and is therefore a [[Propositions|proposition]]). 
- We can universally quantify multi-valued predicates as well. For example, the algebraic statement "There exist values of $x$ and $y$ such that $x = 2^y$" is true (for example $x = 2, y = 1$). This can be written as $\exists x \exists y (x = 2^y)$. 
- If a predicate has more than one variable input, quantifying one of those variables does not produce a proposition, but rather another predicate with unquantified variables. The remaining unquantified variables are said to be *undetermined* while the quantified variables are *bound*. 
- If a predicate has more than one variable input, quantifying *all* the variables produces a [[Propositions|proposition]]. For example "$a+b$ is even" is not a proposition because it is sometimes true and sometimes false, depending on the values of $a$ and $b$. But the statement "For all integers $a$ and $b$, $a+b$ is even" is simply false (because the statement is not true "for all" integers $a$ and $b$, for example $a = 2$, $b=1$). 

## Examples 

The statement "The [[natural number]] $n$ is a perfect square" is a predicate. Let $P(n)$ represent this predicate. Then $\exists n P(n)$ ("There exists a natural number that is a perfect square") is its existentially quantified form. It is a proposition because it has a definite truth value: True, because $n = 4$ is an example. 

The statement "$m$  is a perfect square" is a predicate. If $N(m)$ is this predicate, then $\exists m N(m)$ ("There is a negative integer $m$ that is a perfect square") is its existentially quantified form. It is a predicate with a definite truth value: False, because you cannot get a negative number by squaring another (real) number. 

## Resources 

<iframe src="https://player.vimeo.com/video/600466128?h=2a59394446" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/600466128">Screencast 2.9: Quantification</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Book section: [Quantifiers](https://www.whitman.edu/mathematics/higher_math_online/section01.02.html)
- Video: [Existential quantifiers](https://www.youtube.com/watch?v=OzLorUzIQ1U)