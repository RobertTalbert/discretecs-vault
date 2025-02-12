---
aliases:
  - deductions
  - deduction
  - Deduction
  - deduction rule
tags:
  - logic
created: 2025-01-06
updated:
---
---
## Definition 

> [!tldr] Definition
> A **deduction rule** is an argument form consisting of a collection of [[Propositions|statements]] called the **premises** (plural of the word "premise") and a single statement called the **conclusion**, in which the conclusion is true whenever the premises are all true. In such cases we say the deduction rule is **valid**. 

**Notes**
- The term "conclusion" here is not the same as when we use that term to describe a part of a [[Conditional statements|conditional statement]]. The [[Conditional statements|conclusion]] of a [[Conditional statements|conditional statement]] is simply the [[Atomic and molecular propositions|atomic statement]] that follows the "then" in the phrase "If $A$, then $B$". For a deduction rule, the conclusion can be a [[Atomic and molecular propositions|molecular statement]]. 
- A deduction rule is said to be **invalid** if there is a situation in which all the premises are true but the conclusion is false. 

## Examples and Non-Examples

**Example**: Consider the deduction rule whose premises are the two [[Propositions|statements]] $P \rightarrow Q$ and $P$, and in which the conclusion is $Q$. We sometimes denote this in a table-like form: 

$$\begin{array}{c} P \to Q \\[8pt] P \\[8pt] \overline{\hspace{2cm}} \\[8pt] \therefore Q \end{array}$$
A natural-language version of this deduction rule might go like this: 
- If it's raining, then my windshield wipers will come on. ($P \rightarrow Q$)
- It's raining. ($P$)
- Therefore, my windshield wipers will come on. ($Q$)
To check to see that this deduction rule is valid, make a [[Truth tables|truth table]] that includes all the [[Atomic and molecular propositions|atomic statements]] and a column for each of the premises and the conclusion: 

| $P$ | $Q$ | $P \rightarrow Q$ | Row in which both premises are true |
| --- | --- | ----------------- | ----------------------------------- |
| T   | T   | T                 | ⬅                                   |
| T   | F   | F                 |                                     |
| F   | T   | T                 |                                     |
| F   | F   | T                 |                                     |
 There is only one condition where both premises are true, shown in the first row. And in that row, the conclusion $Q$ is also true. Therefore the deduction rule is valid. In fact, this is a common form of argument known as [modus ponens](https://en.wikipedia.org/wiki/Modus_ponens). 

**Non-Example:** A slight variation on the *modus ponens* argument is this: 
$$\begin{array}{c} P \to Q \\[8pt] Q \\[8pt] \overline{\hspace{2cm}} \\[8pt] \therefore P \end{array}$$
In natural language this might sound like: 
- If it rains ($P$), then the ground is wet ($Q$). 
- The ground is wet ($Q$). 
- Therefore it must have rained ($P$). 
Again to check validity, we make a truth table that includes all the premises and the conclusion. This uses the same truth table as before, but we will check it differently: 

| $P$ | $Q$ | $P \rightarrow Q$ | Rows in which both premises are true |
| --- | --- | ----------------- | ------------------------------------ |
| T   | T   | T                 | ⬅                                    |
| T   | F   | F                 |                                      |
| F   | T   | T                 | ⬅                                    |
| F   | F   | T                 |                                      |
The first and third rows are where both premises ($P \rightarrow Q$ and $Q$) are true. But, in this case the conclusion ($P$) is not always true: In the third row it shows that the conclusion might be false. In natural language, even though both premises could be true (it's true that rain makes the ground wet, and it's true that the ground is wet), the conclusion doesn't necessarily follow - the ground could be wet for other reasons, like a sprinkler or spilled water.

## Resources 

![](https://www.youtube.com/watch?v=K1mTW6VvUHQ)

Other resources: 
- [Resource sheet with more examples, that involve truth tables](https://global.uwi.edu/sites/default/files/bnccde/logic/symboliclogic3a.pdf)
