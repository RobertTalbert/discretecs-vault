---
aliases:
  - conditional statement
  - if-then statement
  - implication
  - Implication
  - hypothesis
  - conclusion
---

---

#logic 
## Definition 

> [!tldr] Definition
> A **conditional statement** is a [[Propositions|proposition]] that has the form "If $A$, then $B$" where $A$ and $B$ are [[Propositions|propositions]]. The proposition $A$ in the "if" part is called the **hypothesis** of the conditional statement, and the proposition $B$ in the "then" part is called the **conclusion**. 
> 
> The conditional statement "If $A$ then $B$" is written in mathematical notation as $A \rightarrow B$. 

Notes:
- Conditional statements need not literally be phrased as "if-then" statements; any phrasing that indicates a conclusion follows from a hypothesis is equivalent. For example, here are five different ways to phrase the conditional statement "If it's snowing, then it's cold": 
	- *Snowing implies that it's cold*.
	- *It's cold whenever it's snowing.*
	- *Snowing is a sufficient condition for it to be cold.*
	- *Being cold is a consequence of it snowing.*
	- *Being cold follows from it snowing.*
	[See this article for more](https://math.stackexchange.com/questions/42042/different-ways-to-express-if-then). 
* We consider the arrow in $P \rightarrow Q$ to be a [[connective]] that joins the [[Propositions|propositions]] $P$ and $Q$. 
* The [[Truth tables|truth table]] for the conditional statement $P \rightarrow Q$ is: 

| $P$ | $Q$ | $P \rightarrow Q$ | 
| -- | -- | ---- |
| T | T | T | 
| T | F | F | 
| F | T | T | 
| F | F | T | 


> [!important] When are conditional statements false? 
> Conditional statements are false only in one case: When the hypothesis is true but the conclusion is false. (That is, the consequence does not follow from the condition.)

* The [[Negation|negation]] of a conditional statement is *not* another conditional statement, rather it is the proposition $P \wedge (\neg Q)$. This is because the truth table for $P \wedge (\neg Q)$ is 

| $P$ | $Q$ | $P \wedge (\neg Q)$ | 
| -- | -- | ---- |
| T | T | F | 
| T | F | T | 
| F | T | F | 
| F | F | F | 

And this has the exact opposite truth values as $P \rightarrow Q$. 

## Examples 

Here are examples of conditional statements with the hypothesis and conclusions indicated: 

| Statement                                                                  | Hypothesis           | Conclusion    |
| -------------------------------------------------------------------------- | -------------------- | ------------- |
| If Bob has pizza, he'll get sick.                                          | Bob has pizza        | Bob gets sick |
| If $x > 3$ then $x^2 > 9$.                                                 | $x > 3$              | $x^2 > 9$     |
| A running time longer than 3 minutes follows from the input being too big. | The input is too big | The running time is longer than 3 minutes              |

Note the last example shows that the hypothesis of the conditional statement doesn't have to appear at the first of the sentence; it is merely the condition that triggers the response, and this can be phrased in different ways.  
## Resources 
<iframe src="https://player.vimeo.com/video/588372005?h=411ac35f76" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/588372005">Screencast 2.3: Conditional statements</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>
Other resources: 
- [Textbook section on conditional statements](https://math.libretexts.org/Courses/SUNY_Schenectady_County_Community_College/Discrete_Structures/01%3A_Introduction_to_Writing_Proofs_in_Mathematics/1.01%3A_Statements_and_Conditional_Statements#:~:text=more%20formal%20definition.-,Definition,true%20whenever%20P%20is%20true.), with practice exercises 