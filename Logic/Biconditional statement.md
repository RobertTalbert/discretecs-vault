---
aliases: [if and only if, biconditional, biconditional statement]
--- 

#logic 

## Definition 

> [!tldr] Definition
> A **biconditional statement** is a [[Propositions|proposition]] that has the form "$A$ if and only if $B$" where $A$ and $B$ are [[Propositions|propositions]]. 
> 
> The biconditional statement  "$A$ if and only if $B$" is written in mathematical notation as $A \leftrightarrow B$. 

Notes:
* We consider the double arrow in $P \leftrightarrow Q$ to be a [[Connectives|connective]] that joins the [[Propositions|propositions]] $P$ and $Q$. 
* The [[Truth tables|truth table]] for the biconditional statement $P \leftrightarrow Q$ is: 

| $P$ | $Q$ | $P \leftrightarrow Q$ | 
| -- | -- | ---- |
| T | T | T | 
| T | F | F | 
| F | T | F | 
| F | F | T | 

- In other words, **biconditional statements are true whenever the two propositions have the same truth value**. 
- The statement $P \leftrightarrow Q$ is [[Logical equivalence|logically equivalent]] to the statement $(P \rightarrow Q) \wedge (Q \rightarrow P)$. That is, the biconditional statement is true if the [[Conditional statements|conditional statement]] $P \rightarrow Q$ and its [[Converse|converse]] are both true, and false otherwise. 
