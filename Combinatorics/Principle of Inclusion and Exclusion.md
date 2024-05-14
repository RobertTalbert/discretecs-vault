---
aliases: [Inclusion-Exclusion Principle, Inclusion-Exclusion, PIE]
--- 

#combinatorics 

## Definition 

> [!tldr] Definition
> The Principle of Inclusion and Exclusion states that if an event $A$ can occur in $m$ ways, and an event $B$ can occur in $n$ ways, and there are $p$ ways for both $A$ and $B$ to happen at the same time, then the number of ways for the event "$A$ or $B$" to happen is $m+n-p$. 

Notes: 
- Informally the Principle of Inclusion and Exclusion says that the number of ways for either $A$ or $B$ to happen equals the number of ways $A$ can happen, plus the number of ways $B$ can happen, **minus the number of ways $A$ and $B$ can happen**. 
- The subtraction is due to the fact that outcomes where $A$ and $B$ happen simultaneously are counted twice if we just add the outcomes of $A$ to the outcomes of $B$. 
- The Principle of Inclusion and Exclusion can be phrased in terms of [[Set|sets]]: If $A$ and $B$ are any two sets, then $|A \cup B| = |A| + |B| - |A \cap B|$. (The vertical bars indicate [[Cardinality|cardinality]]; the symbol $\cup$ is the [[Union|union]]; the symbol $\cap$ is [[Intersection|intersection]].)
- The [[Additive principle]] is really just a special case of the Principle of Inclusion and Exclusion, where the two events are disjoint; in this case you'd just be subtracting off zero, since the [[intersection]] of disjoint sets is empty. 
- The Principle of Inclusion and Exclusion can be extended to three or more events, but the formula gets progressively more complicated. [Go here to learn more](https://artofproblemsolving.com/wiki/index.php/Principle_of_Inclusion-Exclusion#Three_Set_Examples). 

## Example

- **How many [[natural numbers]] between 1 and 1000 (including 1 and 1000) are either even, or are multiples of 3?** First, note that the [[Additive principle]] doesn't apply directly here since being even and being a multiple of 3 are not [[Intersection|disjoint]] events: It's possible for a number to be both even and a multiple of 3, for example the numbers 6 or 30. So the answer to the question is: 

> (The count of even numbers from 1 to 1000) + (The count of multiples of 3 from 1 to 1000) - (The count of numbers that are both even and multiples of 3 from 1 to 1000)

Exactly half of the numbers from 1 to 1000 are even, so there are 500 of those. The number of multiples of 3 in this range is $\lfloor 1000/3 \rfloor = 333$ (divide 1000 by 3 and round down; or just do a direct count using a Python script). In order to be both even and a multiple of 3, a number has to be a multiple of 6; there are $\lfloor 1000/6 \rfloor = 166$ of those in this range. Therefore there are $500 + 333 - 166 = 667$ natural numbers from 1 to 1000 that are either even or multiples of 3. 

The following Python script will verify that count: 
```Python
len([n for n in range(1,1001) if n % 2 == 0 or n % 3 == 0])
```


## Resources 

<iframe src="https://player.vimeo.com/video/618309204?h=17b1d061c9" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/618309204">Screencast 4.1: The Additive Principle and Principle of Inclusion-Exclusion</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Tutorial: [Principle of Inclusion-Exclusion](https://artofproblemsolving.com/wiki/index.php/Principle_of_Inclusion-Exclusion)
