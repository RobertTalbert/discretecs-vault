---
aliases: [truth table, truth tables]
---

#logic

## Definition 

> [!tldr] Definition
> A **truth table** is a table that separates a logical [[Propositions|proposition]] into its [[Atomic and molecular propositions|atomic statements]], lists all possible combination of truth values for those atomic statements, and then determines the truth value of the proposition in each case. 

Notes: 
- If a proposition has $n$ atomic propositions that make it up, its truth table will have $2^n$ rows (not counting a header row), one for each combination of truth values of the atomic propositions. 
- The truth tables for the four basic connectives are: 

[[Negation]] ("not"): 

|  $P$  | $\neg P$ |
|:-----:|:--------:|
| True  |  False   |
| False |        True  |

[[Conjunction]] ("and"): 

| $P$ | $Q$ | $P \wedge Q$ | 
| :--: | :--: | :------: |
| True | True | True | 
| True | False | False | 
| False | True | False | 
| False | False | False | 

[[Disjunction]] ("or"): 

| $P$ | $Q$ | $P \vee Q$ | 
| :--: | :--: | :------: |
| True | True | True | 
| True | False | True | 
| False | True | True | 
| False | False | False | 

[[Conditional statements|Implication]] ("if-then"): 


| $P$ | $Q$ | $P \rightarrow Q$ | 
| :--: | :--: | :------: |
| True | True | True | 
| True | False | False | 
| False | True | True | 
| False | False | True | 

- The entries in a truth table can be any symbol with two states, with one representing True and the other False. For example they can be the words "True" and "False"; or the letters "T" and "F"; or the bits $1$ for True and $0$ for False; and so on. 


## Examples 

To make a truth table for a molecular statement, start by making columns for each of its atomic propositions and rows for all the combinations of truth values of those propositions. Then build the table by making one column for each molecular statement in the main proposition, piece by piece. 

**Example:** Make the truth table for $P \vee (\neg Q)$. First, set up two columns and list all the truth combinations: 

| $P$ | $Q$ |  
| :--: | :--: | 
| True | True | 
| True | False | 
| False | True | 
| False | False | 

Now build the table up piece by piece. Start with a column for $\neg Q$: 

| $P$ | $Q$ | $\neg Q$ | 
| :--: | :--: | :------: |
| True | True | False | 
| True | False | True | 
| False | True | False | 
| False | False | True | 

Now add the column for $P \vee (\neg Q)$ by joining $P$ with $\neg Q$ using a disjunction. The vertical arrows indicate which columns you should focus on: 

| $\stackrel{\Downarrow}{P}$ | $Q$ | $\stackrel{\Downarrow}{\neg Q}$ | $P \vee (\neg Q)$ | 
| :--: | :--: | :------: | :----: | 
| True | True | False | True | 
| True | False | True | True | 
| False | True | False | False | 
| False | False | True | True | 

**Example:** Write the truth table for $(A \wedge B) \rightarrow C$. This proposition has three atomic propositions, so it will have *eight* rows: 

| $A$ | $B$ | $C$ | 
| :---: | :---: | :---: | 
| True | True | True | 
| True | False | True | 
| False | True | True | 
| False | False | True | 
| True | True | False | 
| True | False | False | 
| False | True | False | 
| False | False | False | 

Now build up the main statement first with a column for $A \wedge B$: 

| $\stackrel{\Downarrow}{A}$ | $\stackrel{\Downarrow}{B}$ | $C$ | $A \wedge B$ | 
| :---: | :---: | :---: | :----: | 
| True | True | True | True | 
| True | False | True | False | 
| False | True | True | False |
| False | False | True | False | 
| True | True | False | True | 
| True | False | False | False | 
| False | True | False | False | 
| False | False | False | False | 

Then add the final column for the main proposition $(A \wedge B) \rightarrow C$: 

| $A$ | $A$ | $\stackrel{\Downarrow}{C}$ | $\stackrel{\Downarrow}{A \wedge B}$ | $(A \wedge B) \rightarrow C$ | 
| :---: | :---: | :---: | :----: | :---: | 
| True | True | True | True | True | 
| True | False | True | False | True | 
| False | True | True | False | True | 
| False | False | True | False | True | 
| True | True | False | True | False | 
| True | False | False | False | True | 
| False | True | False | False | True | 
| False | False | False | False | True | 



## Resources

<iframe src="https://player.vimeo.com/video/592797708?h=7fabfc2432" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/592797708">Screencast 2.5: Truth tables</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

<iframe src="https://player.vimeo.com/video/593393012?h=ad4ea15742" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/593393012">Screencast 2.6: Truth tables with intermediate steps</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

<iframe src="https://player.vimeo.com/video/597356440?h=d373ef30bf" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/597356440">Screencast 2.7: More complex truth tables</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>


Other resources: 
- [Truth table generator](https://web.stanford.edu/class/cs103/tools/truth-table-tool/) (Stanford University)
- [Example of truth table generation using Wolfram|Alpha](https://www.wolframalpha.com/input?i=truth+table+%28A+and+B%29+implies+C) 

## Practice 

1. Make up propositions with 2, 3, or even 4 or more atomic propositions in them and a variety of connectives. 
2. Write up the truth table by hand. 
3. Check your work using one of the resources listed above. 

