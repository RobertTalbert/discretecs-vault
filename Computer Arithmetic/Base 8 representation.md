---
aliases: [octal, octal representation, base 8]
--- 

#computer-arithmetic 

## Definition 

> [!tldr] Definition
> An [[Integers|integer]] is written in **base 8** or **octal** format if it consists of a string of the numbers $0$ through $7$ that represent groupings of powers of 8. 

Notes: 
- The first few powers of $8$ are: 

| Power of $8$ | Value |
| :------------: | :-----: |
| $8^0$        | $1$   |
| $8^1$        | $8$   |
| $8^2$        | $64$  |
| $8^3$        | $512$ |
| $8^4$        |  $4096$     |

These are all powers of $2$ as well, since $8 = 2^3$. 
## Examples 

The number $267$ can be written as a sum of powers of $2$ as follows: 
$$267 = 4 \times 64 + 1 \times 8 + 3 \times 1 = 4 \times 8^2 + 3 \times 8^1 + 4 \times 8^0$$
Therefore $267$ in [[Base 10 representation|base 10]], is $413$ in base 8.  A subscript is often used to indicate which base we mean: $267_{10} = 413_{8}$. 

Likewise, the number 24 is $24 = 3 \times 8 = 3 \cdot 8^1 + 0 \times 8^0$. Therefore $24_{10} = 30_8$. 
## Resources 

The first 5 minutes of this video includes more information on octal representation: 
<iframe src="https://player.vimeo.com/video/575939514?h=75dcd68fbc" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/575939514">Screencast 1.2: Base 8 and Base 16 representation of integers</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- [RapidTables web page for converting from base 10 to base 8](https://www.rapidtables.com/convert/number/decimal-to-binary.html)
- [YouTube video tutorial on conversion to octal](https://www.youtube.com/watch?v=ayul1fmZd0Y)
- [Converting from base 10 to base 8 in Excel]([https://smallbusiness.chron.com/convert-decimals-binary-numbers-using-excel-39699.html](https://www.causal.app/formulae/dec2oct-excel)), using the `DEC2OCT` function
## Practice 

1. Generate a random positive [[Integers|integer]]. Start small (1-4) digits at first. [Use this website](https://www.random.org/integers/) to generate random [[integers]]. 
2. Write the [[Integers|integer]] as a sum of powers of 8, then write its octal form. 
3. Check your work using the websites above. 

Some samples are below. 


| Base 10 | Base 8 |
| ------- | ------ |
| 53      | 65     |
| 320     | 500    |
| 688     | 1260   |
| 894     | 1576   |
| 948     | 1664   |
