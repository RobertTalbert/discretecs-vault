---
aliases: [multiplicative principle, multiplication principle, Multiplication Principle]
--- 

#combinatorics

## Definition 

> [!tldr] Definition
> The **multiplicative principle** of counting states that if an event $A$ can occur in $m$ ways, and another event $B$ can occur in $n$ different ways, then the number of ways for $A$ and $B$ to happen simultaneously is $m \cdot n$. 

Notes: 
* The multiplicative principle is used when counting the number of outcomes of a process where the steps in the process are independent of each other and we know the number of outcomes of each step. 
* The multiplicative principle can be extended to more than two events. 

## Examples 

- (*The "license plate" problem*) The license plate numbers in a certain state consist of three letters (A through Z) and three digits (0 through 9). How many possible license plate numbers are there? Think of choosing a license plate number as a six-step process: Choose the first letter, then the second, then the third; then choose the first digit, then the second, then the third. There are $26$ ways to choose each letter (and the choice of a letter in one step doesn't influence the choice in the next step); and there are $10$ ways to choose each digit. So the total number of license plate numbers is $26 \cdot 26 \cdot 26 \cdot 10 \cdot 10 \cdot 10 = 17, 576, 000$. 
- What if no duplicates of either letters or digits were allowed? It's still a six-step process but the number of choices in each step will change. There are 26 choices for the first letter, now 25 for the second, and 24 for the third; likewise there are 10 choices for the first digit, now 9 for the second, and 8 for the third. The total number of license plate numbers is therefore $26 \cdot 25 \cdot 24 \cdot 10 \cdot 9 \cdot 8 = 11,232,000$. 
- How many ways are there to have a license plate that starts with either the letter "Q" or the letter "X"? The multiplicative principle is only partially helpful here because we need to count the number of outcomes of two [[Intersection|disjoint]] choices (starting with a Q versus starting with an X) and so we need the [[Additive principle]]. 


> [!NOTE] Solution to the third example
> Break the problem up by counting the number of ways to start with a Q first, then count the number of ways to start with an X. Once we figure those out, use the [[Additive principle]]. 
> 
> Number of ways to start with a Q: If we start with a Q then there are $26$ choices for the second letter and $26$ choices for the third (we are assuming duplicates are OK), then 10 choices for each digit. The multiplicative principle then says the total number of "Q" license plates is $26^2 \cdot 10^3 = 676,000$. 
> 
> Number of ways to start with an X: It's the same reasoning as starting with a Q, so $676,000$ of these. 
> 
> Since these two outcomes are disjoint and we are counting the ways either one could happen, the Additive Principle applies and the total number of outcomes is $676000 + 676000 = 1,352,000$. 



## Resources 

<iframe src="https://player.vimeo.com/video/618923433?h=b267fa03f6" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/618923433">Screencast 4.2: The Multiplicative Principle</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>


Other resources: 
- Tutorial: [Multiplicative principle](https://www3.nd.edu/~apilking/Math10120/Lectures/Solutions/Topic03.pdf)
