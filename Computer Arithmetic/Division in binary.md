---
aliases: [base 2 division, binary division]
--- 
#computer-arithmetic 
## Process 

> [!tldr] Process
>   If $a$ and $b$ are [[Base 2 representation|base 2]] ([[Base 2 representation|binary]]) [[integers]] and $a \geq b$, to find $a \div b$:
>   First define division of single [[Binary digits and bitstrings|bits]]: $0 \div 1 = 0$, $1 \div 1 = 1$, and division by $0$ is meaningless.  
>   If $a$ and $b$ are larger than single bits, first remove any leading $0$ bits that are on the left. Then, use a modified form of long division: 
> 1. Compare the divisor (the number that is doing the division) with the first digit of the dividend (the number that is being divided). If you can divide by the divisor (possibly with remainder), the first digit of the quotient (the result) is $1$. Otherwise it is $0$. 
> 2. Append the next digit to the dividend and repeat this process, appending digits until you get $1$. 
> 3. Once you have a $1$ in the quotient, multiply the divisor by $1$ (which is just making a copy of the divisor) and write it underneath the dividend. 
> 4. Then use [[Subtraction in binary|binary subtraction]] to subtract the divisor from the part of the dividend that it sits under. 
> 5. Bring down the next digit of the dividend and repeat this process. 
> 6. Continue the process of finding digits of the quotient and performing [[Subtraction in binary|binary subtraction]] until no more division can be done. 
> 7. The remainder of this division process will be either $0$ or $1$; $0$ if the divisor evenly divides the last step in the subtraction process or $1$ if it doesn't. 

## Examples 

Divide $11011$ by $10$. (Note, in [[base 10]] this is $27$ divided by $2$, so the result should be a quotient of $13$ and a remainder of $1$.)
1. The first digit of the dividend is $1$. The number $10$ is bigger than this, so $10$ does not divide $1$. Therefore the first bit of the quotient is $0$. 
2. Append the next digit of the dividend to get $11$. The number $10$ does go into $11$, once with a remainder of $1$. So the next bit in the quotient is $1$, and we put a copy of the divisor below this block of digits: $11$ and $10$ under it. 
3. Use [[Subtraction in binary|binary subtraction]] to get $11 - 10 = 1$. 
4. Bring down the next digit of the dividend to get $10$. The divisor, $10$, goes into this once with no remainder. So the next bit in the quotient is $1$; and we put a copy of the divisor below $10$. Subtracting, we get $10 - 10 = 0$. 
5. Bring down the next digit of the dividend to get $01$. The divisor, $10$, is bigger than this, so no division takes place. 
6. Bring down the next digit of the dividend to get $011$. The number $10$ does go into $011$, once with a remainder of $1$. So the next bit in the quotient is $1$, and we put a copy of the divisor below this block of digits: $11$ and $10$ under it.  
7. Use [[Subtraction in binary|binary subtraction]] to get $011 - 10 = 1$. 
8. There are no more bits in the dividend. So the quotient is $1101$ and there is a remainder of $1$. 

This is nearly impossible to understand in verbal form. Here is the actual long division process as an image: 

![[binary-division.jpg|200]]
## Resources 
<iframe title="vimeo-player" src="https://player.vimeo.com/video/581300654?h=af558ca917" width="640" height="360" frameborder="0"    allowfullscreen></iframe>

Other resources: 
- [Binary division calculator with steps](https://madformath.com/calculators/digital-systems/binary-arithmetic/binary-division-calculator-with-steps/binary-division-calculator-with-steps)
- [Binary calculator](https://www.calculator.net/binary-calculator.html) (no steps shown)

## Practice 

To practice this concept: Just make up pairs of random positive integers and convert to binary (or make up pairs of random [[Binary digits and bitstrings|bitstrings]]). Then divide them (smaller into larger). Then check your work by either using the [binary arithmetic calculator](https://www.calculator.net/binary-calculator.html) or by converting the answer to [[Base 10 representation|base 10]] and seeing if it matches what you should get if you multiplied the original integers together in [[Base 10 representation|base 10]]. 