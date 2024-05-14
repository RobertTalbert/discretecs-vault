---
aliases: [k-permutation, k-permutations]
--- 

#combinatorics 

## Definition 

> [!tldr] Definition
> A **$k$-permutation** is a rearrangement of a group of $k$ objects taken from a larger group of objects. The number of $k$-permutations of objects taken from a group of $n$ objects is notated $P(n,k)$. 

**Notes**: 
- $k$-permutations are similar to [[Permutation|permutations]], in fact they are the same idea except $k$-permutations involve selection from a larger set in addition to rearranging the selection. 
- If the items in the larger set are all distinct, the following formula for $P(n,k)$ comes directly from the [[Multiplicative principle]] and its application to [[License plate problem|license plate problems]]:
$$P(n,k) = \frac{n!}{(n-k)!}$$
## Example and non-example

* **How many three-letter substrings can be made from the (six letter) word "GUITAR"?** Since all the letters in the word are different, the number is 
$$P(6,3) = \frac{6!}{(6-3)!} = \frac{6!}{3!} = 6 \cdot 5 \cdot 4 = 120$$
- The formula is unnecessary for the previous problem because you can think of it as a [[License plate problem|license plate problem]]: Consider the three-character substring as three empty slots to be filled. There are 6 ways to fill the first slot, 5 to fill the second, and 4 to fill the third. Then use the [[Multiplicative principle]] to find the result. 
- **Non-example:** In a pizza restaurant with 10 toppings available, how many ways can you order a pizza with 4 toppings (and no double-toppings)? The answer is *not* $P(10,4) = 10!/6! =  5040$ because this considers rearrangements of toppings on a pizza as completely different pizzas. For example the selection *pepperoni, sausage, mushrooms, pineapple* would be counted differently from the selection *sausage, pineapple, pepperoni, mushrooms* even though these are the same pizza -- so there is an overcount. In this case we are not creating *rearrangements* of toppings, we are just selecting four toppings from a set of 10 and not caring about what order in which we make the selection. So the correct answer is given by the [[Binomial coefficient|binomial coefficient]]: 
$$\binom{10}{4} = \frac{10!}{4! \cdot 6!} = 210$$
- In the non-example, you can also reason through it to say that $P(10,4)$ overcounts by a factor equal to the number of ways to rearrange a selection of four things. Since double-toppings aren't allowed, that number is $4!$ and so the correct count is $P(10,4)/4! = 210$. 
## Resources 

<iframe src="https://player.vimeo.com/video/626473882?h=92e0a801af" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/626473882">Screencast 4.8: Rearrangements and k-permutations</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- Tutorial: https://zipcon.net/~swhite/docs/math/probability/counting.html See "Permutations of _k_ items taken from _n_ items". 
