---
updated: 2025-01-06
aliases:
  - binary subtraction
  - base 2 subtraction
---
---

#computer-arithmetic 

## Process 

> [!tldr] Process
> If $a$ and $b$ are [[Base 2 representation|base 2]] ([[Base 2 representation|binary]]) [[integers]] and $a \geq b$, to find $a-b$:
> 1. Start in the ones ($2^0$) place and subtract the [[Binary digits and bitstrings|bits]] there: $0 - 0 = 0$, $1-1 = 0$, $1-0 = 1$; and if we encounter $0-1$ then **borrow** $1$ from the twos ($2^1$) place to make the $0$ into $10$, then subtract to get $10 - 1 = 1$. 
> 2. Subtract the [[Binary digits and bitstrings|bits]] in the twos ($2^1$) place. Again, $0 - 0 = 0$, $1-1 = 0$, $1-0 = 1$; and if we encounter $0-1$ then **borrow** $1$ from the fours ($2^2$) place to make the $0$ into $10$, then subtract to get $10 - 1 = 1$. 
> 3. Continue this process of subtracting, borrowing from the next higher place if needed, until we reach the left end of the [[Binary digits and bitstrings|bitstring]]. 

Notes: 
- It's also possible to "subtract" $b$ from $a$ by finding the [[Base 2 representation|binary]] form of $b$ using [[two's complement]] notation, then using [[Addition in binary|binary addition]] to add this to $a$. However there are potential issues with the bit size; the procedure outlined above has no such restrictions. 

## Examples 

Subtract the [[Base 2 representation|base 2]] integers $1101$ and $1010$. That is, find $1101 - 1010$. Note that in base 10, this would be $13 - 10$, so the answer should be $3$ which is $11_2$. 
1. Subtract [[Binary digits and bitstrings|bits]] in the ones ($2^0$) place: $1-0 = 1$. 
2. Subtract [[Binary digits and bitstrings|bits]] in the twos ($2^1$) place: We have $0-1$ so we borrow $1$ from the fours ($2^2$) place to make the $0$ into a $10$, then subtract: $10 - 1 = 1$. 
3. Subtract [[Binary digits and bitstrings|bits]] in the fours ($2^2$) place: This would have been $1-1$ except we borrowed in the previous step, so the first $1$ is now a $0$. Therefore we have $0-0$ which is $0$. 
4. Subtract [[Binary digits and bitstrings|bits]] in the eights ($2^3$) place: $1-1 = 0$. 
Therefore $1101 - 1010 = 0011$ which is $11$. That's what we expected. 

## Resources 

<iframe src="https://player.vimeo.com/video/579560863?h=6eb2a3d0de" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/579560863">Screencast 1.5: Subtraction in binary</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- [Binary arithmetic calculator](https://www.calculator.net/binary-calculator.html)
- [Tutorial on binary subtraction](https://byjus.com/maths/binary-subtraction/)
- Video: [How to add and subtract binary numbers](https://www.youtube.com/watch?v=C5EkxfNEMjE)

## Practice 

To practice this concept: Just make up pairs of random positive integers and convert to binary (or make up pairs of random [[Binary digits and bitstrings|bitstrings]]). Then subtract them. Then check your work by either using the [binary arithmetic calculator](https://www.calculator.net/binary-calculator.html) or by converting the answer to [[Base 10 representation|base 10]] and seeing if it matches what you should get if you subtracted the original integers together in [[Base 10 representation|base 10]]. 
