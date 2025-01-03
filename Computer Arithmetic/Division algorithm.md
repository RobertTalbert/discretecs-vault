---
tags:
  - computer-arithmetic
aliases:
  - The Division Algorithm
  - division algorithm
---
---

## Definition 

> [!tldr] Definition
> The **Division Algorithm** is a mathematical [[Theorem|theorem]] that states the following: 
> 
> For any two positive integers $a$ and $b$, there exist unique integers $q$ (the *quotient*) and $r$ (the *remainder*) such that $a = bq + r$ and $0 \leq r < b$. 

Notes: 
- The Division Algorithm as a [[Theorem]] does not state how the integers $q$ and $r$ are to be computed; it only asserts that they exist, and there is only one such pair that satisfies both of the requirements ($a = bq + r$ and $0 \leq r < b$). 
- As stated above, the Division Algorithm gives the quotient and remainder when dividing $a$ by $b$ (that is, $a \div b$). 
- The final requirement in the Division Algorithm statement, asserts that the remainder in the integer division process has to be strictly smaller than the divisor. This has important implications in computer algorithms involving division. 
- The actual process of finding the quotient and remainder is embodied in [long division](https://www.mathsisfun.com/long_division.html), which we learned in grade school. 
- In Python, the quotient when dividing $a$ by $b$ is computed using the operator `//` for [[integer division]]. The remainder when dividing $a$ by $b$ is computed using the operator `%` which is the [[Modulus operator|modulus operator]]. 

## Examples and Non-Examples

- If $a = 30$ and $b = 7$, then the quotient $q$ is $4$ and the remainder $r$ is $2$ because $30 = 7 \times 4 + 2$ and $0 \leq 2 < 7$. In Python, ``30 // 7 = 4`` and ``30 % 7 = 2`` . 
- If $a = 10$ and $b = 22$, then the quotient $q$ is $0$ and the remainder is $r = 22$ because $22 = 0 \times 100 + 22$ and $0 \leq 22 < 100$. So note, even if the number we are dividing is smaller than the number we are dividing by, the Division Algorithm still applies. 
## Resources 

The first 7 minutes of this video give more background on the Division Algorithm:
<iframe src="https://player.vimeo.com/video/583046507?h=ef4d7d314f" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/583046507">Screencast 1.8: The Division Algorithm and the modulus operator</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- [Refresher on long division](https://www.mathsisfun.com/long_division.html) 
