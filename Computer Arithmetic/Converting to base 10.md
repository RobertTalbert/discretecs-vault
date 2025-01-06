---
aliases:
  - base 10 conversion
updated: 2025-01-06
---
---

#computer-arithmetic 

## Process

> [!summary] To convert an [[Integers|integer]] *from* any number base *to* [[Base 10 representation|base 10]]: 
> - Make a note of the base that the [[Integers|integer]] is using ([[Base 2 representation|base 2]], [[Base 8 representation|base 8]], [[Base 16 representation|base 16]], etc.)
> - Write out the [[Integers|integer]] as a sum of copies of powers of the base, using the digits as multipliers
> - Perform the arithmetic that results in [[Base 10 representation|base 10]]. 

To convert *from* [[Base 10 representation|decimal]] *to* a different base, see the article on the [[base conversion algorithm]]. 

To convert from a *non-[[Base 10 representation|decimal]] base* to *another non-decimal base* (e.g. [[Base 10 representation|decimal]] to [[Base 8 representation|octal]]), see the article on non-[[Base 10 representation|decimal]] base conversions. 

## Examples 

Example: Convert $100111_{2}$ to [[Base 10 representation|base 10]]. 

- The base is 2. 
- Use the digits to write the [[Integers|integer]] as a sum of powers of 2: $100111_{2} = 1 \times 2^5 + 0 \times 2^4 + 0 \times 2^3 + 1 \times 2^2 + 1 \times 2^1 + 1 \times 2^0$. 
- Do the arithmetic: $1 \times 2^5 + 0 \times 2^4 + 0 \times 2^3 + 1 \times 2^2 + 1 \times 2^1 + 1 \times 2^0 = 32 + 4 + 2 + 1 = 39$ in [[Base 10 representation|base 10]]. 

Example: Convert $BD7_{16}$ to [[Base 10 representation|base 10]]. 

- The base is 16. 
- Use the digits to write the [[Integers|integer]] as a sum of powers of 16: $BD7_{16} = 11 \times 16^2 + 13 \times 16^1 + 7 \times 16^0$. 
- Do the arithmetic: $11 \times 16^2 + 13 \times 16^1 + 7 \times 16^0 = 11 \times 256 + 13 \times 16 + 7 \times 1 = 3031$ in [[Base 10 representation|base 10]]. 



## Resources 

This video starting at 7:45 has more examples of converting [[Base 2 representation|binary]] to [[Base 10 representation|decimal]]: 
<iframe src="https://player.vimeo.com/video/575905500?h=463d7f680d" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/575905500">Screencast 1.1: Base 10 and Base 2 representation of integers</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

This video starting has more examples of converting octal (at 2:45) and hexadecimal (at 5:24) to decimal: 
<iframe src="https://player.vimeo.com/video/575939514?h=75dcd68fbc" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/575939514">Screencast 1.2: Base 8 and Base 16 representation of integers</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

This video starting at the 4:18 mark has more on [[base 16 representation]]: <iframe src="https://player.vimeo.com/video/575939514?h=75dcd68fbc" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/575939514">Screencast 1.2: Base 8 and Base 16 representation of integers</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- [Binary to decimal converter](https://www.rapidtables.com/convert/number/binary-to-decimal.html)
- [Octal to decimal converter](https://www.rapidtables.com/convert/number/octal-to-decimal.html) 
- [Hexadecial to decimal converter](https://www.rapidtables.com/convert/number/hex-to-decimal.html)


