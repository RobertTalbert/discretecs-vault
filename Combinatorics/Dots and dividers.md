---
aliases: [dots and dividers, stars and bars]
--- 

#combinatorics 

## Definition 

> [!tldr] Definition
> The **dots and dividers** method is an approach to counting the number of ways to distribute identical objects to a group of recipients. The basic outline of the method is: 
> 1. Represent each object being distributed as a "dot".
> 2. Represent the *change from one recipient to another* as a "divider". 
> 3. Each distribution is now representable as a sequence of dots and dividers, which can be translated into [[Binary digits and bitstrings|bitstrings]] in which each dot is a `0` and each divider is a `1`. 
> 4. The number of those bitstrings, and hence the number distributions, can then be counted with the [[Binomial coefficient|binomial coefficient]]. 

**Notes:**
- This method goes by other names including *stars and bars*; *balls and bars*;  *sticks and stones*; and *balls and urns*. 

## Examples 

> [!example]
> **Problem:** How many ways are there to distribute ten identical 20-dollar bills to three children? 
> 
> **Solution:** Model each distribution using dots and dividers with each bill represented by a dot, and each change between children as a divider. For example, giving the first child 2 bills, the second child 5 bills, and the third child 3 bills would be represented as: `**|*****|***`. Likewise the diagram `****||******` represents a distribution where the first child gets 4 bills, the second child gets none, and the third child gets 6. Each diagram corresponds to a 12-bit [[Binary digits and bitstrings|bitstring]] that has [[Weight of a bitstring|weight]] 2 because there are always 2 dividers no matter what the distribution. There are $\binom{12}{2} = 66$ of these. 

> [!example]
> **Problem**: How many nonnegative integer solutions are there to the equation $x + y + z + w = 15$? 
> 
> **Solution**: This is the same problem as distributing 15 identical objects to four different people, so we can model each solution as a dots-and-dividers diagram. For example $x = 1$, $y = 4$, $z = 8$, $w = 2$ is a solution and can be represented by the diagram `*|****|********|**`. There are 15 dots and 3 dividers, so each diagram can be thought of as an 18-bit string with weight 3. There are $\binom{18}{3} = 816$ of these. 

## Resources 

<iframe title="vimeo-player" src="https://player.vimeo.com/video/626749580?h=336008db3a" width="640" height="360" frameborder="0"    allowfullscreen></iframe>

Other resources: 
- Video: [Stars and bars counting](https://www.youtube.com/watch?v=epY_8lcKxCU)
- Tutorial: [Ball-and-urn](https://artofproblemsolving.com/wiki/index.php/Ball-and-urn)