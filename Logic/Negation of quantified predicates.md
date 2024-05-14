---
aliases: [negation of predicates]
--- 

#logic 

## Facts 

> [!tldr] Facts
> Suppose $P(x)$ is a predicate. Then: 
> - The negation of its existentially quantified form $\exists x P(x)$ is $\forall x (\neg P(x))$. 
> - The negation of its universally quantified form $\forall x P(x)$ is $\exists x (\neg P(x))$. 
> 
> That is: $\neg (\exists x P(x)) = \forall x (\neg P(x))$ and $\neg (\forall x P(x)) = \exists x (\neg P(x))$. 

Notes: 
- In English, this is saying: 
	- The negation of "There exists an $x$ such that $P(x)$ is true", is the statement "For all $x$, $P(x)$ is false."
	- The negation of "For all $x$, $P(x)$ is true", is the statement "There exists an $x$ such that $P(x)$ is false."
- Note that in each case we not only negate the predicate, but change the quantifier. 
- Negating a quantified [[multivariable predicate]] follows the same principles. 

## Examples and Non-Examples

Here are some quantified predicates with their negations, in regular English: 

| Quantified predicate                                                 | Symbolic form    | Negation of symbolic form | Negation in English                                                                                                                    |
| -------------------------------------------------------------------- | ---------------- | ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| Every MTH 225 student has red hair.                                  | $\forall x P(x)$ | $\exists x (\neg P(x))$   | There is at least one MTH 225 student who does not have red hair.                                                                      |
| There is a student in your section of MTH 225 who is a millionaire. | $\exists x P(x)$ | $\forall x (\neg P(x))$   | Every student in your section of MTH 225 is not a millionaire. *Or:* None of the students in your section of MTH 225 are millionaires. |
| For every real number $x$, there is a real number $y$ such that $x = 2^y$. | $\forall x \exists y P(x,y)$ | $\exists x \forall y (\neg P(x,y))$ | There is a real number $x$ such that $x \neq 2^y$ for any real number $y$. 
## Resources 

<iframe src="https://player.vimeo.com/video/600490216?h=74ce90b919" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/600490216">Screencast 2.10: Negating quantified statements</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Book section: [Quantifiers and negations](https://math.libretexts.org/Courses/SUNY_Schenectady_County_Community_College/Discrete_Structures/02%3A_Logical_Reasoning/2.04%3A_Quantifiers_and_Negations) (with practice exercises)
- Video: [Predicate logic and quantifier negation](https://www.youtube.com/watch?v=gyoqX0W-NH4)
