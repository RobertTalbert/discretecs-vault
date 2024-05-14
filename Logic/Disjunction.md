---
aliases: [disjunction]
--- 

#logic

## Definition 

> [!tldr] Definition
> A **disjunction** is a logical [[Connectives|connective]] joining two [[Propositions|propositions]], which results in a new proposition that is true only when one or both of the two propositions is true. It is the logical version of the english word "or". The notation for a disjunction is the symbol $\vee$, and we pronounced $A \vee B$ as "$A$ or $B$". 

Notes: 
- The [[Truth tables|truth table]] for the disjunction $A \vee B$ is: 

| $A$   | $B$   | $A \vee B$ |
| ----- | ----- | ------------ |
| True  | True  | True         |
| True  | False | True        |
| False | True  | True        |
| False | False | False             |

Again, $A \vee B$ is true only when *either* $A$ *or* $B$, **or both**, is true. 

- Because we include the condition that $A$ and $B$ are both true as a situation where $A \vee B$ is true, we refer to disjunction sometimes as an *inclusive "or"*. Compare this with the [[Exclusive OR]]. 
- In Python, the disjunction is implemented by just the word `or`. 
- In other languages, the disjunction is frequently indicated by `||` ("double pipe").  
## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/585958504" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 2.2: Logical connectives"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

Other resources: 
- Tutorial: [Logical OR operator](https://learn.microsoft.com/en-us/cpp/cpp/logical-or-operator-pipe-pipe?view=msvc-170) (Microsoft)
