---
aliases: [codomain]
--- 

#sets-functions 

## Definition 

> [!tldr] Definition
> The **codomain** of a [[Function|function]] is the [[Set|set]] consisting of all allowable outputs of that function. In standard function notation, if $f: A \rightarrow B$ is a function then the set $B$ is the codomain. 

Notes: 
- The codomain of $f$ contains the [[Range|range]] of the function as a [[Subset|subset]], but the two are not necessarily equal. See examples below. 
- Informally we can think of the codomain as specifying the "data type" of the outputs. For example the ceiling function $ceil: \mathbb{R} \rightarrow \mathbb{Z}$ that takes a real number and rounds it up, has a codomain of $\mathbb{Z}$ which indicates that the outputs are of "type integer". 

## Examples 

- The function $f: \mathbb{R} \rightarrow \mathbb{R}$ defined as the formula $f(x) = x^2$ has codomain equal to $\mathbb{R}$, the set of all real numbers. (This is also its [[Domain|domain]].)
- The function $p: \mathbb{N} \rightarrow \mathbb{N}$ defined by assigning $n$ to the $n$th digit of $\pi$. So $p(0) = 3$, $p(1) = 1$, $p(2) = 4$, $p(3) = 1$, etc. has codomain equal to the [[natural numbers]] (same as its [[domain]]). 
- The function from $A = \{-2,0,3,5\}$ to $B = \{-4,-3,4\}$ shown in the diagram below has a codomain of $\{-4,-3,4\}$: 
![[simple-function-diagram.png|300]]
- The (Python) function shown below takes a positive integer and returns a list of all of its positive divisors. For example `divisors(18) = [1,2,3,6,9,18]`. The domain in this case is the set of all positive integers, and the codomain is the set of all *lists of* positive integers. (That is, the outputs have a "data type" of lists containing positive integers.)
```python
def divisors(n): 
    return [i for i in range(1,n+1) if n % i == 0]
```

## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/614432178?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 3.8: Functions"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

- Video: [Domain, Codomain, and Range](https://www.youtube.com/watch?v=H10d0NF-gXU)
- Tutorial: [Domain, Range, and Codomain](https://www.mathsisfun.com/sets/domain-range-codomain.html)

