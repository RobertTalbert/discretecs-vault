---
aliases: [sequence, sequences]
--- 

#recursion-induction 

## Definition 

> [!tldr] Definition
> A **sequence** is an ordered list of numbers. 

Notes: 
* The main difference between a sequence and a [[Set|set]] is that sequences are ordered while sets aren't. 
* Sequences can also contain duplicate elements while [[Set|sets]] cannot. For example $1, 2, 1, 2, 1, 2, \dots$ is an acceptable sequence. 
* Sequences typically have a *first* element, followed by a second, third, fourth, etc. elements. Typically we [zero-index](https://stringfestanalytics.com/seen-zero-based-indexing/) a sequence, meaning we refer to the first item in the sequence as having "position 0". 
* If we use variables to represent terms in a sequence, we write $a_0, a_1, a_2, a_3, \dots$ (The letter $a$ can be replaced with other letters; but notice the index of the term appears as a subscript.) 
* Sequences can be expressed as explicit lists, [[Recursion|recursively]], or as [[Closed formula|closed formulas]]. See below for examples. 

## Examples and Non-Examples

Here are some sequences: 

- $1, 1, 2, 3, 5, 8, 13, 21, 34, \dots$ is the [[Fibonacci sequence]]. 
- $1, 3, 6, 10, 15, 21, \dots$ is the sequence of triangular numbers. 
- $3, 1, 4, 1, 5, 9, \dots$ is the sequence of digits of $\pi$. 
- The sequence $2, 3, 5, 9, 17, 33, \dots$ can also be given as a [[Closed formula|closed formula]]: $f(n) = 1 + 2^n$ where $n \geq 0$. 
- The sequence $2, 4, 10, 22, 52, 118, \dots$ can be expressed [[Recursion|recursively]] as follows: $a_0 = 2$, $a_1 = 4$, and if $n \geq 2$ then $a_n = 3a_{n-2} + a_{n-1}$. This is an example of a [[Recurrence relation|recurrence relation]].  

## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/635492325?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 5.1: Sequences"></iframe></div>

Other resources: 
- Tutorial: [Sequences](https://www.mathsisfun.com/algebra/sequences-series.html)
- [Khan Academy unit on sequences](https://www.khanacademy.org/math/algebra/x2f8bb11595b61c86:sequences)
