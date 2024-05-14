---
aliases: [induction, mathematical induction, Induction, inductive hypothesis]
--- 

#recursion-induction 

## Definition 

> [!tldr] Definition
> **Mathematical induction** is a [[proof]] technique used when proving that a [[Predicate|predicate]] $P(n)$ (whose [[Domain|domain]] is the set of all [[Natural numbers|natural numbers]]) is true for all natural numbers or for some specified [[Subset|subset]]. It is especially applicable if the predicate involves [[Recursion|recursion]]. Induction proofs follow a three-step **framework**: 
> 1. (*Base case*) Establish, by direct computation or demonstration, that $P(n)$ is true for the smallest value of $n$ for which it is claimed to be true. That is, establish that the base case leads to a true statement.  
> 2. (*Inductive hypothesis*) Assume that $P(k)$ is true for some random, undisclosed value of $k$. 
> 3. (*Inductive step*) Prove that $P(k+1)$ is true, using a combination of the inductive hypothesis, the recursion involved in the predicate, previously-proven results, and so on. 

**Notes**: 
- This general framework is sometimes known as *weak induction*. Other forms of induction are possible, including [strong induction](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/resources/lecture-3-strong-induction/), [structural induction](https://www.cs.umd.edu/class/summer2016/cmsc250/files/slides/structuralInduction.pdf), and [transfinite induction](https://mathworld.wolfram.com/TransfiniteInduction.html). 
- The base case is often $n = 0$ but not always. Check the statement being proven for the smallest case.

## Examples 

Consider the Python function
```python
def f(n): 
	if n == 0: return 3
	else: return 2*f(n-1)
```

By playing with examples, we see this function returns the [[sequence]] $3, 6, 12, 24, 48, \dots$. So we might conjecture that **For all natural numbers $n$, $f(n) = 3 \cdot 2^n$.** 

Here is an example of just setting up the framework for a proof of this conjecture: 

> [!NOTE] Framework for an induction proof
> First of all, the predicate $P(n)$ in this case is the claim that "$f(n)$ as computed by the Python code is equal to $3 \cdot 2^n$". 
> 
> **Base case:** We need to demonstrate directly that the predicate is true in the smallest possible case, which here is $n=0$. Well, on the one hand $f(0)$ is 3 because the Python code explicitly says to return 3 when the input is 0. On the other hand $3 \cdot 2^0 = 3 \cdot 1 = 3$. Since the two are equal, the predicate is true in the base case. 
> 
> **Inductive hypothesis:** Assume that $f(k) = 3 \cdot 2^k$ for some natural number. 
> 
> **Inductive step:** We would now need to prove that $f(k+1) = 3 \cdot 2^{k+1}$. 

And, here is a complete proof of the conjecture: 

> [!proof]
> We will show that $f(n)$ as computed by the Python function is equal to $3 \cdot 2^n$ for all natural numbers $n$. We will prove this using mathematical induction. 
> 
> First, in the base case where $n=0$: The Python function returns $3$ in this case. And on the other hand, $3 \cdot 2^0 = 3 \cdot 1 = 3$. The code and the formula return the same result, so the base case holds. 
> 
> Now assume that for some $k > 0$, $f(k)$ as computed by the Python code equals $3 \cdot 2^k$. We want to show that $f(k+1)$ as computed by the code equals $3 \cdot 2^{k+1}$. 
> 
> (Note: We can assume that $k$ is strictly greater than $0$ because the case where $k=0$ was already handled in the base case.)
> 
> Since $k > 0$, if we enter $k+1$ into the Python code, it will return $2 \cdot f((k+1)-1)$. This is equal to $2 \cdot f(k)$ because in the parentheses, $k+1-1$ is equal to $k$. By assumption (in the inductive hypothesis) $f(k)$ equals $3 \cdot 2^k$. So the result of entering in $k+1$ is 
> $$2 \cdot f(k) = 2 \cdot \left( 3 \cdot 2^k\right) = 3 \cdot 2^{k+1}$$
> Therefore we've shown that entering in $k+1$ gives $3 \cdot 2^{k+1}$. This is what we wanted to show, so we can conclude that $f(n) = 3 \cdot 2^n$ for all natural numbers $n$. ⬛

Here are three complete examples of proof by mathematical induction: 

> [!NOTE] **Claim:** For all natural numbers $n$, the number $n^3 + 2n$ is divisible by $3$. 
> 
> **Proof:** First, to prove the base case, if $n=0$ then we have $0^3 + 2(0)$ which equals $0$. This is a multiple of $3$ because $0 = 3 \times 0$. Therefore the base case is proven. 
> 
> Now assume that for some natural number $k$, $k^3 + 2k$ is a multiple of 3. We want to show that $(k+1)^3 + 2(k+1)$ is a multiple of 3. Expand this out to get: 
> 
> $$\begin{align}
> (k+1)^3 + 2(k+1) &= (k^3 + 3k^2 + 3k + 1) + (2k + 2) \\
>    &= (k^3 + 2k) + 3k^2 + 3k + 3
> \end{align}
> $$
> Now we already assumed that $k^3 + 2k$ was a multiple of 3, and clearly the last three terms are multiples of 3 because 3 is a factor on each. Therefore $(k+1)^3 + 2(k+1)$ is a sum of multiples of 3, which makes the entire expression a multiple of 3. 
> 
> That ends the proof.   

> [!NOTE] **Claim:** The sum $1 + 2 + 3 + \dots + n$ is equal to $\dfrac{n(n+1)}{2}$ for all $n \geq 1$. 
> 
> **Proof:** First, to prove the base case, note the smallest case for which this statement is claimed to be true is $n=1$. In this case, the sum has only one term and is equal to $1$. On the other hand $\dfrac{1(1+1)}{2} = \frac{2}{2} = 1$. Since these are equal, the base case holds. 
> 
> Now assume the induction hypothesis: $1 + 2 + 3 + \cdots + k = \dfrac{k(k+1)}{2}$ for some $k$. 
> 
> We want to prove that $1 + 2 + 3 + \cdots k + (k+1) = \dfrac{(k+1)(k+1+1)}{2}$. 
> 
> On the left, we have $1 + 2 + 3 + \cdots k + (k+1)$. If we group the first $k$ terms together we have $(1 + 2 + 3 + \cdots + k) + (k+1)$ and the inductive hypothesis says that the sum inside the parentheses is $\frac{k(k+1)}{2}$. Therefore the left side is $\frac{k(k+1)}{2} + k+1$. Using some algebra, this is equal to $\dfrac{k^2 + k}{2} + \dfrac{2k+2}{2}$. Adding the fractions gives $\dfrac{k^2 + 3k + 2}{2}$. Factoring the numerator gives $\dfrac{(k+1)(k+2)}{2}$. And this is equal to $\dfrac{(k+1)(k+1+1)}{2}$ which is what we wanted to show. 
> 


> [!NOTE] Claim: Every set with $n$ elements has $2^n$ subsets. 
> The base case is $n=0$. A set with zero elements is the [[Empty set|empty set]], and there is only one subset of this, namely the empty set itself. So the base case holds. 
> 
> Now assume that for some $k > 0$, every set with $k$ elements has $2^k$ subsets. We want to show that every set with $k+1$ elements has $2^{k+1}$ subsets. 
> 
> Suppose that $A$ is a set with $k+1$ elements, which we can take to be just the numbers $1$ through $k+1$. That is, assume $A = \{1, 2, 3, \dots, k+1\}$.  (We can assume that $A$ is this specific set because there would be a [[Bijective|bijection]] between this set and any other set with $k+1$ elements.)  Look at the set $B = \{1, 2, \dots, k\}$. Each subset of $A$, the parent set, is one of two things: 
> 
> - A subset of $B$, or 
> - One of the subsets of $B$ [[Union|union]] with the set $\{k+1\}$. 
> 
> Since $B$ has $k$ elements, then by the inductive hypothesis, $B$ has $2^k$ subsets. Therefore there are $2^k$ subsets of $A$ that fall into the first category (they are just subsets of $B$) and another $2^k$ subsets in the second category (they are a subset of $B$ with the number $k+1$ added in). That's $2 \cdot 2^k$ sets in all, which equals $2^{k+1}$, and this is the full number of subsets of $A$.  ⬛




## Resources 

* [Text/web tutorial on induction](https://hackmd.io/QtgTZTnRQkeQYoe8BObF4A?view)

Below are several induction videos made for MTH 210 (Communicating in Mathematics) at Grand Valley State University. They are dated but possibly useful. 

- [The traveler and the strange staircase](https://www.youtube.com/watch?v=9LwAtbXSB3A&list=PL2419488168AE7001&index=51&pp=iAQB)
- [Mathematical induction part 1](https://www.youtube.com/watch?v=JTj6ID4-084&list=PL2419488168AE7001&index=52&pp=iAQB)
- [Mathematical induction part 2](https://www.youtube.com/watch?v=1H0gg3fMYVA&list=PL2419488168AE7001&index=53&pp=iAQB)
- [Mathematical induction Example with integer division](https://www.youtube.com/watch?v=ayX6PxB3z40&list=PL2419488168AE7001&index=54&pp=iAQB)
- [Mathematical induction Example with an inequality](https://www.youtube.com/watch?v=upzROTcbAnk&list=PL2419488168AE7001&index=55&pp=iAQB)
- [Mathematical induction Example from Calculus](https://www.youtube.com/watch?v=GQ9fUZxmN8I&list=PL2419488168AE7001&index=56&pp=iAQB)
