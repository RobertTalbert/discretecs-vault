---
aliases: [binomial coefficient]
--- 

#combinatorics 

## Definition 

> [!tldr] Definition
> For each [[Integers|integer]] $n \geq 0$ and for each integer $k$ with $0 \leq k \leq n$, the **binomial coefficient**, denoted $\displaystyle{\binom{n}{k}}$ and pronounced "$n$ choose $k$", is a number that represents the number of ways to select $k$ objects from a group of $n$ distinct objects. 

**Notes:**

- Please note, $\binom{n}{k}$ is *not* a fraction. For example $\binom{10}{2}$ does not equal $5$. 
- The binomial coefficient is sometimes notated as $C(n,k)$. 
- The binomial coefficient $\binom{n}{k}$ also represents: 
	- The number of [[Binary digits and bitstrings|bitstrings]] with length $n$ and [[Weight of a bitstring|weight]] $k$ 
	- The number of $k$-element [[Subset|subsets]] of an $n$-element set 
	- The coefficient on $x^ky^{n-k}$ in the expansion of $(x+y)^n$
- The binomial coefficient $\binom{n}{k}$ can be computed [[Recursion|recursively]] when $n \geq 1$ and $k \geq 1$, using the [[Recurrence relation|recurrence relation]]: 
$$\binom{n}{k} = \binom{n-1}{k-1} + \binom{n-1}{k}$$
- The binomial coefficient $\binom{n}{k}$ can be computed directly using the closed formula
$$\binom{n}{k} = \frac{n!}{k! (n-k)!}$$
Here, the exclamation point in $n!$ is the [[Factorial|factorial function]]. 

## Examples 

- Because $\displaystyle{\binom{n}{k}}$ is the number of ways to select $k$ objects from a group of $n$ objects, $\displaystyle{\binom{5}{5}} = 1$. There is only one way to take a group of 5 objects and select all 5. The closed formula above also says this, but remember the binomial coefficient solves a counting problem. 
- More generally, $\displaystyle{\binom{n}{n}} = 1$ for all $n \geq 0$. 
- For the same reason, $\displaystyle{\binom{n}{0}} = 1$ for any $n \geq 0$ because there is only one way to select nothing from a group of $n$ objects. 
- **How many 8-bit strings are there with exactly 5 `1` bits?** This is asking, *how many 8-bit strings have [[Weight of a bitstring|weight]] 5?* The answer is $\displaystyle{\binom{8}{5} = \frac{8!}{5! \cdot 3!}} = 56$. 
- **How many ways are there to choose three letters from the alphabet A..Z without duplication if we don't care about the ordering of the letters?** This is the same question as: **How many three-element subsets are there of a 26-element set?** The answer to both is $\displaystyle{\binom{26}{3} = \frac{26!}{3! \cdot 23!}} = 2600$. 

## Resources 

The following videos cover the binomial coefficient from first principles. These build on each other, so each video beyond the first references all the ones before it, so watching them out of order could lead to confusion: 
- [Counting subsets and strings](https://vimeo.com/714228019)
- [Counting $k$-element subsets](https://vimeo.com/714225614)
- [Counting $n$-bit strings of weight $k$](https://vimeo.com/618985119)
- [Why counting subsets and counting bitstrings are the same](https://vimeo.com/714227663)
- [The Binomial Coefficient](https://vimeo.com/621554165)


Other resources: 
- Tutorial: [Use the Binomial Theorem](https://courses.lumenlearning.com/waymakercollegealgebra/chapter/use-the-binomial-theorem/) 
