---
aliases: [recursion, recursively, recursive]
--- 

#recursion-induction
## Definition 

> [!tldr] Definition
> **Recursion** is the process of computing or constructing an object using simpler versions of itself. A process that exhibits recursion is called *recursive*. 
> 
> A recursive process needs two parts to be fully specified: 
> 1. A *base case* (or base cases) that gives the computation or construction directly without recursion, and 
> 2. A *recursive step* consisting of a set of rules for computing or building all other cases out of simpler cases, eventually terminating in the base case. 

Notes: 
- Without the base case, a recursive process would enter an [infinite regress](https://en.wikipedia.org/wiki/Infinite_regress) where computations would continue but never end. 

## Examples

### The [[Fibonacci sequence]]

The *Fibonacci sequence* is a sequence of [[integers]] defined recursively as follows: 
- Base case: The first two Fibonacci numbers, $F_0$ and $F_1$ are defined directly: We declare $F_0 =1$ and also $F_1 = 1$. 
- Recursive step: All other Fibonacci numbers are computed as *the sum of the previous two Fibonacci numbers*. That is, for $n \geq 2$, $F_n = F_{n-1} + F_{n-2}$. 

The Fibonacci sequence therefore starts with $F_0 = 1$ and $F_1 = 1$. Then $F_2 = F_1 + F_0 = 1 + 1 = 2$. Then $F_3 = F_2 + F_1 = 2 + 1 = 3$. Then $F_4 = F_3 + F_2 = 3 + 2 = 5$. And so on. The first 20 numbers in the sequence are: 
$$1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610, 987, 1597, 2584, 4181, 6765, \dots$$

Here is a recursive Python function for computing the $n$th Fibonacci number: 
```python
def fib(n):
	if n == 1 or n == 2: return 1
	else: 
		return fib(n-1) + fib(n-2)
```
(Warning, this function is extremely slow for inputs above 20.)

### Summing a list of numbers

Suppose `L` is a list of numbers. We can define the sum of the list, `sum(L)`, recursively using the length of the list: 
- Base case: If the length of `L` is $0$ then `sum(L)` is defined to be $0$. If the length of `L` is $1$, then `sum(L)` is defined to be just the single number in the list. 
- Recursive step: If the list has length $2$ or greater, then select the first element in the list and call it `a`. Then, `sum(L)` is `a`, plus the `sum` of the list consisting of `L` with `a` removed. 

Thus, for example, `sum([8,6,7,5])` would be computed like this: 

$$\begin{align*}
\text{sum}([8,6,7,5]) &= 8 + \text{sum}([6,7,5]) \\
&= 8 + (6 + \text{sum}([7,5])) \\
&= 8 + (6 + (7 + \text{sum}([5]))) \\
&= 8 + 6 + 7 + 5 \\
&= 26
\end{align*}
$$
Here is a recursive Python function that does this: 
```python
def sum_rec(L):
    if len(L) == 0: return 0
    elif len(L) == 1: return L[0] 
    else: 
        return L[0] + sum_rec(L[1:])
```

### Other examples

Many other examples of recursion are found throughout mathematics and computing, including the [[binomial coefficient]]. 

## Resources 

<iframe src="https://gvsu.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=568ac590-eb95-4fb6-b329-b08100f1ef15&autoplay=false&offerviewer=true&showtitle=true&showbrand=true&captions=false&interactivity=all" height="405" width="720" style="border: 1px solid #464646;" allowfullscreen allow="autoplay" aria-label="Panopto Embedded Video Player"></iframe>


Other resources: 
- Video: [Recursion simply explained with code examples](https://www.youtube.com/watch?v=m1Fjdnj_Mds)
- Video: [Learn recursion in 8 minutes](https://www.youtube.com/watch?v=u8Xam9EsqXQ)
- Video : [5 simple steps for solving any recursive problem](https://www.youtube.com/watch?v=ngCos392W4w)

