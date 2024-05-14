---
aliases: [geometric sequence, geometric]
--- 

#recursion-induction 

## Definition 

> [!tldr] Definition
> A [[sequence]] of numbers is said to be **geometric** if each number in the sequence is a fixed multiple of the previous term. Put differently, a sequence is geometric if the ratio of any two consecutive terms is constant. 

Notes: 
- We say that geometric sequences "grow with a constant ratio" or "constant multiple". 
- Geometric sequences have a [[Recursion|recursive]] definition by letting $a_0$ be the first term of the sequence, then $a_n = r a_{n-1}$ where $r$ is the common ratio. 

## Examples and Non-Examples

- The sequence $1, 2, 4, 8, 16, 32, \dots$ is geometric because each term is $2$ times the previous term. 
- The sequence $3.1, 9.61, 29.791, 92.3521, 286.29151, 887.503681, \dots$ is geometric because each item is $3.1$ times the previous term. It's easier to tell this if you look at the ratios instead. If you take any two consecutive terms and divide them, the result is always $3.1$: $9.61/3.1 = 3.1$, $29.791/9.61 = 3.1$, and so on. 
- The sequence $3.1, 6.2, 9.3, 12.4, 15.5, 18.6, \dots$ is *not* geometric because there is not a common ratio between the terms. For example $6.2/3.1 = 2$ but $9.3/6.2 \neq 2$. (This is an [[arithmetic sequence]].)

## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/638676941?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 5.3: Arithmetic and geometric sequences"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

Other resources: 
- Tutorial: [Geometric sequences and sums](https://www.mathsisfun.com/algebra/sequences-sums-geometric.html)
- Video: [Introduction to geometric sequences](https://www.youtube.com/watch?v=pXo0bG4iAyg) 