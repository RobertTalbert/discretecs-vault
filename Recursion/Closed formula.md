---
aliases: [closed formula, closed formulas]
--- 

#recursion-induction 

## Definition 

> [!tldr] Definition
> A **closed formula** for a [[Sequence|sequence]] is a mathematical formula for producing the $n$th term of the sequence using a fixed finite number of operations on the index $n$. 

Notes
- Closed formulas can be thought of as a [[Function|function]] whose [[Domain|domain]] is $\mathbb{N}$ (the set of all [[Natural numbers]]). The input to such a function is the index of the sequence. 
- Closed formulas are one way of viewing a sequence, along with [[Recurrence relation|recurrence relations]]. 
- There are specific methods for finding closed formulas for a sequence if the sequence is [[Arithmetic sequence|arithmetic]] or [[Geometric sequence|geometric]]. 
## Examples and Non-Examples

- The closed formula $a_n = 3n+1$ produces the sequence $1, 4, 7, 10, 13, \dots$ (assuming the sequence is zero-indexed). 
- The closed formula $b_n = \dfrac{n(n+1)}{2}$ produces the sequence $0, 1, 3, 6, 10, 15, \dots$ 
- The sequence $1, 2, 4, 8, 16, 32, \dots$ can be produced with the closed formula $c_n = 2^n$. 
- The formula $d_n = d_{n-1} + n$ is *not* a closed formula for a sequence because of the presence of $d_{n-1}$. This is a [[Recursion|recursive]] definition of a sequence that cannot be determined using just a fixed finite set of operations on $n$. 

## Resources 

- Video: [Determine a closed formula for a given sequence](https://www.youtube.com/watch?v=4YxqncJCack)
