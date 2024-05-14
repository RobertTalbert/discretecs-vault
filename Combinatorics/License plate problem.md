---
aliases: [license plate problems, license plate problem]
--- 

#combinatorics 

## Definition 

> [!tldr] Definition
> The **license plate problem** is a general category of counting problems motivated by counting the number of license plates possible when given a certain way of making them. (Examples are below.) 

**Notes**: 
* The license plate problem is a typical and common use of the [[Multiplicative principle]] and of [[k-Permutation|k-permutations]]. 
## Examples 

- **A certain state makes license plates with three letters A:Z followed by three digits 0:9. How many license plates are possible?** Visualize the license plate as six empty slots: 
![[licenseplate.png]]
There are 26 ways to fill in each of the first three slots, and 10 ways to fill in each of the last three slots. Applying the [[Multiplicative principle]], the number of license plates is $26^3 \cdot 10^3$. 
- **How many 6-bit strings are there that either start on the left with `00` or end on the right with `11`?** Visualize the 6-bit string as a license plate with six slots. If we require the string to start with `00`, then the first two slots are taken and there are 2 ways to fill in the other 4, giving a total of $2^4$ ways to start with `00`. Similarly, there are $2^4$ ways to end in `11`. Note that these conditions are not [[Intersection|disjoint]] because we can have a bit string that starts with `00` and ends in `11`; a string like that would leave the middle two slots open, so there are $2^2 = 4$ ways to have such a string. Therefore by the [[Principle of Inclusion and Exclusion]], the number of strings that either start with `00` or end in `11` is $2^4 + 2^4 - 2^2 = 28$. 


## Resources 

- Tutorial: [Permutation license plate problem](https://www.beatthegmat.com/permutation-license-plate-problem-t5270.html)
