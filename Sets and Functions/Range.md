---
aliases: [range]
--- 

#sets-functions 
## Definition 

> [!tldr] Definition
> The **range** of a [[Function|function]] is the [[Set|set]] consisting of all actual outputs of that function. 

Notes: 
- The range of $f$ is a [[Subset|subset]] of, but is not necessarily equal to, the [[Codomain|codomain]] of $f$. See below for examples where they are different. 
- Whereas the [[Codomain|codomain]] is a general set of "potential" outputs of $f$ (the "data types" of the output), the range is the set of *actual, specific outputs* that are produced by the function. 

## Examples and Non-Examples

- The ceiling function $ceil: \mathbb{R} \rightarrow \mathbb{Z}$ that takes a real number and rounds it up, has a range of $\mathbb{Z}$ because every [[Integers|integer]] actually occurs as the output of some input. (For example, $19$ is the output if you "plug in" $18.4$.) In this case the range and [[Codomain|codomain]] are equal. 
- The function $f: \mathbb{R} \rightarrow \mathbb{R}$ defined as the formula $f(x) = x^2$ has [[Codomain]] equal to $\mathbb{R}$, the set of all real numbers. But its *range* is the set of all *nonnegative* real numbers because it is impossible to square a real number to get a negative output. (And, every nonnegative number actually occurs as the output of something, for example $19$ is the output we get when we plug in $x = \sqrt{19}$. )
- The function $g: \{0,1,2\} \rightarrow \{a,b,c\}$ given explicitly by $g(0) = a$, $g(1) = a$, $g(2) = c$ has [[Codomain]] $\{a,b,c\}$ but the range is just $\{a,c\}$ because only $a$ and $c$ are actually outputs. 


## Resources 


<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/614432178?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 3.8: Functions"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

- Video: [Domain, Codomain, and Range](https://www.youtube.com/watch?v=H10d0NF-gXU)
- Tutorial: [Domain, Range, and Codomain](https://www.mathsisfun.com/sets/domain-range-codomain.html)

