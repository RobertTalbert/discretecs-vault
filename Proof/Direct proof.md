---
aliases:
  - direct proof
tags:
  - proof
created: 2024-06-13
---

---
## Definition 

> [!tldr] Definition
> A **direct proof** is a [[Proof|proof]] applied specifically to a [[Conditional statements|conditional statement]] which is structured as follows: 
> 1. Assume that the [[Conditional statements|hypothesis]] of the conditional statement is true; 
> 2. Then use definitions, computations, previously-proven results, or basic facts to explain why the [[Conditional statements|conclusion]] of the conditional statement is true. 

Notes: 
- A direct proof uses the logic of the [[Conditional statements|conditional statement]] to structure the argument: According to the [[Truth tables|truth table]] for $P \rightarrow Q$, the statement is true when $P$ is false; so we can begin the argument by assuming that $P$ is true. Then it only requires to show that $Q$ must also be true in that condition. 

## Examples and Non-Examples


> [!NOTE] Proof involving even and odd integers
> **Prove: If $n$ is an even integer, then $n^2$ is also even.** 
> 
> **Proof:** We use a direct proof. First, assume that $n$ is an [[Even and odd integers|even]] integer. 
> 
> Since $n$ is even, we can write it as $n = 2k$ where $k$ is another integer. (This is the definition of "[[even]]".) Now look at $n^2$: Since $n = 2k$, we know that $n^2 = (2k)^2$, which means $n^2 = 4k^2$ (using basic algebra to expand $(2k)^2$). We can factor off a $2$ from this to get $n^2 = 2(2k^2)$. Now since $k$ is an integer, $k^2$ is also an integer because of [[Closure of the integers|closure]]; and therefore $2k^2$ is an integer also because of [[Closure of the integers|closure]]. Therefore we have shown there exists an integer, namely $2k^2$, such that $n^2$ is 2 times that integer. This shows that $n^2$ is even, which is what we wanted to show. ◾


> [!NOTE] Proof involving [[Divisibility|divisibility]]
> **Prove: If $a,b,$ and $c$ are integers and $a|b$ and $b|c$, then $a|c$.** 
> 
> **Proof:** Assume the hypothesis, which says that $a|b$ and $b|c$. Using the definition of [[Divisibility|divisibility]], we can then say that there exist integers $x$ and $y$ such that $b = ax$ and $c = by$. We want to show that there is an integer $z$ such that $c = az$.
> 
 




> Since $b = ax$ (wemake a substitution into $c = b[](Divis) to get $c = (ax)y$. The [[Properties of arithmetic|associative property]] then says that $c = a(xy)$. Now since $x$ and $y$ are both integers, $xy$ is also an integer because of [[closure]]. Therefore we have shown that there is an integer $z$, namely $z= xy$, such that $c$ is $a$ times that integer. Therefore $a | c$ by the definition of [[Divisibility|divisibility]]. ◾
> 
 


## Resources 

![](https://www.youtube.com/watch?v=H8LLINU6ebY)

![](https://www.youtube.com/watch?v=1tCOucLfdh0)

![]()
There are a lot more videos with proof examples at the [Grand Valley State University Communicating in Mathematics playlist](https://www.youtube.com/playlist?list=PL2419488168AE7001). 



