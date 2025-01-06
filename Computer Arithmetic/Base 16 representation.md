---
aliases:
  - hexadecimal
  - base 16
  - hexadecimal representation
  - base 16 representation
updated:
---

--- 

#computer-arithmetic 

## Definition 

> [!tldr] Definition
> An [[Integers|integer]] is written in **base 16** or **hexadecimal** format if it consists of a string of the numbers $0$ through $9$ and letters $A$ through $F$ that represent groupings of powers of 16. 

Notes: 

- In hexadecimal, the letter $A$ represents the [[Base 10 representation|base 10]] number $10$; $B$ represents $11$; $C$ represents $12$; $D$ represents $13$; $E$ represents $14$; and $F$ represents $15$. 
- The alphabetical digits are needed to have more than ten copies of a power of 16. 
- The first few powers of 16 are: $16^0 = 1$, $16^1 = 16$, $16^2 = 256$, $16^3 = 4096$. These are all powers of 2 as well, since $16= 2^4$. 

## Examples 

The number $2670$ can be written as a sum of powers of $16$ as follows: 
$$2670 = 10 \times 256 + 6 \times 16 + 14 \times 1 = 10 \times 16^2 + 6 \times 16^1 + 14 \times 16^0$$
Using the multipliers in front of the powers of $16$ and replacing $10$ and $14$ with $A$ and $E$ respectively, we get 
$$2670 \ \text{base 10}  = A6E \ \text{base 16}$$
A subscript is often used to indicate which base we mean: $2670_{10} = A6E_{16}$. 

Likewise, the number 2561 is $$10 \times 256 + 0 \times 16 + 1 \times 1$$so $2561_{10} = A01_{16}$. 

## Resources 
This video starting at the 4:18 mark has more on base 16 representation: <iframe src="https://player.vimeo.com/video/575939514?h=75dcd68fbc" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/575939514">Screencast 1.2: Base 8 and Base 16 representation of integers</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- [RapidTables web page for converting from base 10 to base 16](https://www.rapidtables.com/convert/number/decimal-to-hex.html)
- [Another decimal to hexadecimal converter](https://www.binaryhexconverter.com/decimal-to-hex-converter)
- [Converting from base 10 to base 2 in Excel](https://smallbusiness.chron.com/convert-decimals-binary-numbers-using-excel-39699.html), using the `DEC2HEX` function

## Practice 

1. Generate a random positive integer. Start small (1-4) digits at first. [Use this website](https://www.random.org/integers/) to generate random integers. 
2. Write the integer as a sum of powers of 16, then write its hexadecimal form. 
3. Check your work using the websites above. 
