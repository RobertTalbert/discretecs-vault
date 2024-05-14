---
aliases: [universal quantifier, universally quantified]
--- 

#logic
## Definition 

> [!tldr] Definition
> A [[Predicate|predicate]] is **universally quantified** when we assert that the predicate is true for all values of one or more of its variables. A **universal quantifier** is a logical operator that declares that the predicate is true for all values of a variable. If $P(x)$ is a predicate, then the statement "For all values of $x$, $P(x)$ is true" is its universally quantified form. Symbolically we write this as $\forall x P(x)$. 

Notes: 
- Whereas the single-variable predicate $P(x)$ is not a [[Propositions|proposition]] because its truth value depends on the input $x$, its universally quantified form $\forall x P(x)$ is a proposition with a definite truth value. For example, the statement "The integer $n$ is even" is a predicate that is sometimes true and sometimes false; the quantified form "For every integer $n$, $n$ is even" is definitely false (and is therefore a [[Propositions|proposition]]). 
- We can universally quantify multi-valued predicates as well. For example, the familiar "Commutative Property" of addition from arithmetic says: "For every number $x$ and every number $y$, $x+y = y+x$" and can be written as $\forall x \forall y (x+y = y+x)$. 
- If a predicate has more than one variable input, quantifying one of those variables does not produce a proposition, but rather another predicate with unquantified variables. The remaining unquantified variables are said to be *undetermined* while the quantified variables are *bound*. 
- If a predicate has more than one variable input, quantifying *all* the variables produces a [[Propositions|proposition]]. For example "$a+b$ is even" is not a proposition because it is sometimes true and sometimes false, depending on the values of $a$ and $b$. But the statement "For all integers $a$ and $b$, $a+b$ is even" is simply false (because the statement is not true "for all" integers $a$ and $b$, for example $a = 2$, $b=1$). 

## Examples 

The statement "The [[natural number]] $n$ is a perfect square" is a predicate. Let $P(n)$ represent this predicate. Then $\forall n P(n)$ ("Every natural number is a perfect square") is its universally quantified form. It is a proposition because it has a definite truth value: False, because it's not the case that every natural number is a perfect square. 

The statement "There are $2^n$ [[Binary digits and bitstrings|bitstrings]] of length $n$" is a predicate. Let $S(n)$ represent it. Then $\forall n S(n)$ ("For each $n$, there are $2^n$ bitstrings of length $n$") is its universally quantified form. It is a proposition because it has a definite truth value: True, in this case. 

## Resources 

<iframe src="https://player.vimeo.com/video/600466128?h=2a59394446" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/600466128">Screencast 2.9: Quantification</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Book section: [Quantifiers](https://www.whitman.edu/mathematics/higher_math_online/section01.02.html)
- Video: [Universal quantifiers](https://www.google.com/search?sxsrf=AB5stBjEVnxJWiG-LgYv4giV85pYYdzW1Q:1691162063555&q=universal+quantifier&tbm=vid&source=lnms&sa=X&ved=2ahUKEwjQ2bjQpcOAAxX1kYkEHTzkAr4Q0pQJegQICRAB&biw=1388&bih=1107&dpr=2#:~:text=Universal%20Quantifiers%20%2D%20YouTube,com%20%E2%80%BA%20watch)