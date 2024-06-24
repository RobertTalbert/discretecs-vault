---
aliases:
  - proof by contradiction
  - indirect proof
  - Proof by contradiction
tags:
  - proof
created: 2024-06-24
updated: 2024-06-24
---
---
## Definition 

> [!tldr] Definition
> An **indirect proof**, also called a **proof by contradiction**, is a [[Proof|proof]] of a [[Conditional statements|conditional statement]] in which the entire [[Negation|negation]] of the conditional statement is assumed to be true, and then a sequence of logical steps leads to a contradiction of a known fact or previously-proven result. 

Notes: 
- Recall that the [[Negation|negation]] of the conditional statement $P \rightarrow Q$ ("If $P$, then $Q$") is $P \wedge (\neg Q)$ ("$P$ and not $Q$"). 
- Therefore the first step in an indirect proof is to assume *two* statements: The original hypothesis ($P$) and the negation of the conclusion ($\neg Q$). 
- By assuming the negation of the original conditional statement and then showing that this negation leads to a contradiction, we show that the negation of the original statement is false -- therefore the original statement is true. 
- The fact that we assume two statements at the beginning of an indirect proof makes indirect proofs often very effective. 
- The tradeoff, is that there is usually no direct path to the contradiction that needs to be shown. Often the contradiction is quite subtle. 
- Indirect proof is often useful when the hypothesis of the conditional statement contains a "positive" statement but the conclusion contains a negation. 
- Indirect proof can also be used on statements that are not conditional; see example below. 
- [Some mathematicians reject the entire concept of indirect proof](https://math.stackexchange.com/questions/111878/why-is-it-considered-unlikely-that-there-could-be-a-contradiction-in-zf-zfc)on logical grounds. And many times, an indirect proof can be expressed more simply as a [[Proof by contraposition|proof by contraposition]]. 

## Examples

**Prove: For any real number $x$, if $x^3 - x > 0$ then $x > -1$.

Note: This statement was proven using [[Proof by contraposition|proof by contraposition]] in another article. You can compare the two proofs and see which one seems simpler and easier to understand. Both are valid. 

**Proof:** We use an indirect proof here. So for the sake of finding a contradiction, assume that $x^3 - x > 0$ but also that $x \leq -1$. 

Using algebra, factor $x^3 - x$ into $x(x+1)(x-1)$. We have assumed that $x(x+1)(x-1) > 0$. Now we have also assumed that $x \leq -1$, so the first and third terms of the expression on the left are both negative, so their product is positive. Therefore since $x(x+1)(x-1) > 0$, it must be that $x + 1 > 0$. This means that $x > -1$. But this contradicts the second assumption that $x \leq -1$. Therefore 




> [!NOTE] Proof about non-existence
> 
> **Prove: There are no integers $a$ and $b$ for which $18a + 6b = 1$.** 
> 
> Note: This is not a conditional statement. But an indirect proof is still useful -- this line of reason is often helpful when proving the *non-existence* of something, as we are doing here. 
> 
> **Proof:** We use an indirect proof here. So assume the negation of the statement: That is, there *are* integers $a$ and $b$ for which $18a + 6b = 1$. Dividing both sides of this equation by $6$, we get $3a + b = \frac{1}{6}$. But this is a contradiction, because since $a$ and $b$ are both integers, $3a + b$ must also be an integer due to [[Closure of the integers|closure]]. But $1/6$ is not an integer, and an integer cannot equal a non-integer. Therefore it cannot be the case that there are integers $a$ and $b$ for which $18a + 6b = 1$. ◼

## Resources 

(video)

Other resources: 
- 

## Practice 
