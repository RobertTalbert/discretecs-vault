---
aliases: [additive principle, addition principle, Addition Principle]
--- 

#combinatorics

## Definition 

> [!tldr] Definition
> The **additive principle** of counting states that if an event $A$ can occur in $m$ ways, and an event $B$ can occur in $n$ ways, and there is no way for $A$ and $B$ to happen at the same time, then the event "$A$ or $B$" can occur in $m+n$ ways. 

Notes: 
* If it *is* possible for $A$ and $B$ to occur at the same time, the number of ways that the event "$A$ or $B$" can happen is given by the [[Principle of Inclusion and Exclusion]]. 
* The Additive Principle can be extended to more than two events.For example, if $A$, $B$, and $C$ are events and no two of them can happen at the same time, and the number of outcomes of each are $m$, $n$, and $p$, then the number of ways $A$ or $B$ or $C$ could occur is $m + n + p$. 

## Examples and Non-Examples

- Suppose a university's student ID number system assigns students a random five-digit number. How many ID numbers end in an odd number (1,3,5,7,9)? There are five odd numbers that could work as the ending digit, and only one can actually happen. So we can count the number of ways the ID could end in a 1, the number of ways it could end in a 3, and so on. For each possible odd ending, there are 10000 possible choices for the first four digits (for example 00001, 00011, 00021, ..., 99991). So the total number of options is $5 \times 10000 = 50,000$. (Note this makes sense, because the total number of ID's possible at all is 100,000 and exactly half of those will end in an odd number.)
- Using the same student ID setup, how many ID numbers either start with an odd number *or* end in an odd number? The Additive Principle doesn't apply here, because the events are not [[Intersection|disjoint]]; it's possible for an ID number to both start and end in an odd number, like 58831. So we need the [[Principle of Inclusion and Exclusion]] for this. 


## Resources 

<iframe title="vimeo-player" src="https://player.vimeo.com/video/618309204?h=17b1d061c9" width="640" height="360" frameborder="0"    allowfullscreen></iframe>

Other resources: 
- Wikipedia article: [Addition principle](https://en.wikipedia.org/wiki/Addition_principle)
