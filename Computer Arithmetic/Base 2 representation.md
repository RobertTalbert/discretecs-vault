---
aliases: [binary, binary representation, base 2, base 2 representation]
--- 

#computer-arithmetic 

## Definition 

> [!tldr] Definition
> An [[Integers|integer]] is written in **base 2** or **binary** format if it consists of a string of the numbers $0$ and $1$, called **[[Binary digits and bitstrings|binary digits]]** or "**[[Binary digits and bitstrings|bits]]**",  that represent groupings of powers of 2. 

Notes: 
- A group of 8 bits is known as a **byte**. 
- Every positive integer can in fact be written as a sum of powers of 2 and in only one way. This fact can be proven using [[
## Examples 

The number $267$ can be written as a sum of powers of $2$ as follows: 
$$267 = 256 + 8 + 2 + 1 = 2^8 + 2^3 + 2^1 + 2^0$$
Using $0$ to pad this sum with groups that are not used and $1$ multiplied to groups that are use, this becomes: 
$$267 = 256 + 8 + 2 + 1 = 1 \cdot 2^8 + 0 \cdot 2^7 + 0 \cdot 2^6 + 0 \cdot 2^5 + 0 \cdot 2^4 + 1 \cdot 2^3 + + 0 \cdot 2^2 + 1 \cdot 2^1 + 1 \cdot 2^0$$
The resulting string of $0$'s and $1$'s, read left-to-right, is the binary representation of 267: 
$$267 \ \text{base 10} = 100001011 \ \text{base 2}$$
A subscript is often used to indicate which base we mean: $267_{10} = 100001011_{2}$. 

Likewise, the number 24 is $24 = 16 + 8 = 1 \cdot 2^4 + 1 \cdot 2^3 + 0 \cdot 2^2 + 0 \cdot 2^1 + 0 \cdot 2^0$. Therefore $24_{10} = 11000_2$. 
## Resources 
This video starting at the 3:00 mark has more on binary representation: 
<iframe src="https://player.vimeo.com/video/575905500?h=463d7f680d" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/575905500">Screencast 1.1: Base 10 and Base 2 representation of integers</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- [RapidTables web page for converting from base 10 to base 2](https://www.rapidtables.com/convert/number/decimal-to-binary.html)
- [Calculator.net page, includes conversion from base 10 to base 2 and vice versa](https://www.calculator.net/binary-calculator.html)
- [Converting from base 10 to base 2 in Excel](https://smallbusiness.chron.com/convert-decimals-binary-numbers-using-excel-39699.html), using the `DEC2BIN` function
## Practice 

1. Generate a random positive integer. Start small (1-4) digits at first. [Use this website](https://www.random.org/integers/) to generate random integers. 
2. Write the integer as a sum of powers of 2, then write its binary form. 
3. Check your work using the websites above. 

Some samples are below. 

| Base 10 | Base 2   |
| ------- | -------- |
| 248     | 11111000 |
| 130     | 10000010 |
| 135     | 10000111 |
| 255     | 11111111 |
| 214     | 11010110 |
