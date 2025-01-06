---
aliases:
  - binary multiplication
  - base 2 multiplication
updated: 2025-01-06
---
---


#computer-arithmetic 

## Process 

> [!tldr] Process
>  If $a$ and $b$ are [[Base 2 representation|base 2]] ([[Base 2 representation|binary]]) [[integers]] and $a \geq b$, to find $a \times b$:
>  1. Multiply $a$ by the ones ($2^0$) digit in $b$. This will result either in a copy of $a$, or a row of zeroes. 
>  2. Underneath the result of the previous step, place a padding $0$ on the right. Then multiply $a$ by the twos ($2^1$) digit in $b$. This will result either in a copy of $a$, or a row of zeroes. 
>  3. Underneath the result of the previous step, place two padding $0$'s on the right. Then multiply $a$ by the fours ($2^2$) digit in $b$. This will result either in a copy of $a$, or a row of zeroes. 
>  4. Continue this process, adding an extra padding $0$ on the right each time, until you use the leftmost bit of $b$. 
>  5. Use [[Addition in binary|binary addition]] to add all the resulting rows together. 

## Examples 

Multiply $1101$ by $101$. In [[Base 10 representation|base 10]] this is $13$ times $5$, so the answer should be $65$ or $1000001$. 
1. Multiply $1101$ by the ones ($2^0$) digit in $101$ which is $1$. This produces a copy of $1101$. 
2. Pad on the right with a single $0$ and multiply $1101$ by the twos ($2^1$) digit of $101$. This is a $0$, so the result is $00000$. 
3. Pad on the right with two zeroes and multiply $1101$ by the fours ($2^2$) digit of $101$. This is a $1$, so the result is $110100$ (a copy of $1101$ along with the two padding zeroes). 
4. There are no more [[Binary digits and bitstrings|bits]] in $b$ to multiply by, so now add all the results above in [[Base 2 representation|binary]]: $1101 + 00000 + 110100$. The result is $1000001$ as expected. 
## Resources 

<iframe src="https://player.vimeo.com/video/580457312?h=b1d9b0e518" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/580457312">Screencast 1.6: Multiplication in binary</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- [Binary arithmetic calculator](https://www.calculator.net/binary-calculator.html)
- Video: [Multiplying in binary](https://www.khanacademy.org/math/algebra-home/alg-intro-to-algebra/algebra-alternate-number-bases/v/binary-multiplication) (Khan Academy)
- [Tutorial on binary multiplication](https://www.cuemath.com/numbers/binary-multiplication/)

## Practice 

To practice this concept: Just make up pairs of random positive [[integers]] and convert to [[Base 2 representation|binary]] (or make up pairs of random [[Binary digits and bitstrings|bitstrings]]). Then multiply them. Then check your work by either using the [binary arithmetic calculator](https://www.calculator.net/binary-calculator.html) or by converting the answer to [[Base 10 representation|base 10]] and seeing if it matches what you should get if you multiplied the original [[integers]] together in [[Base 10 representation|base 10]]. 