---
aliases:
  - two's complement
updated: 2025-01-06
---

#computer-arithmetic 

## Definition/Process 

> [!tldr] Process
> Two's complement is a method of representing a *negative* [[Integers|integer]] in [[Base 2 representation|binary]]. To put a negative [[Integers|integer]] in two's complement notation: 
> 1. Decide on the number of [[Binary digits and bitstrings|bits]] to use for the representation. (This often depends on the architecture of the computer system, e.g. an 8-bit system or a 64-bit system.) The number of [[Binary digits and bitstrings|bits]] to use must be greater than the length of the [[Base 2 representation|binary]] representation of the positive version of your number. 
> 2. Take the negative number in [[Base 10 representation|base 10]] and write its *positive* version in [[Base 2 representation|base 2]] (using the [[Base conversion algorithm|base conversion algorithm]]), padding the front of the bit string with extra 
> 3. Flip all the [[Binary digits and bitstrings|bits]] in this [[Base 2 representation|binary]] integer -- change all `0`s to `1`s and vice versa. 
> 4. Using [[Addition in binary|binary addition]], add `1` to this [[Base 2 representation|binary]] integer. 
> 
> The result is the two's complement representation of the original negative integer. 
>

Notes: 
- Other forms of representing negative integers in binary exist besides two's complement. [This page gives a summary](https://www.geeksforgeeks.org/representation-of-negative-binary-numbers/). 

## Examples 

Represent $-42$ in binary using two's complement and 8-bit representation. 

1. The positive version $42$ is $101010$ in binary, and since we are using 8-bit representation we pad this with two extra `0` bits to get $00101010$. 
2. Flip the bits to get $11010101$. 
3. Using [[Addition in binary|binary addition]], add $1$ to this, to get $11010110$. 

Therefore $-42_{10} = 11010110_2$ using two's complement notation. 

Represent $-300$ in two's complement notation. Notice this time we cannot use 8-bit representation because the positive version of this number, 300, is $100101100$ which has 9 bits. So we must use at least 9 bits to represent $-300$. Let's pick a computer-friendly number, 16. 

1. The positive version $300$ is $100101100$, which when padded with `0` bits to make it 16 bits long is $0000000100101100$. 
2. Flip all the bits to get $1111111011010011$. 
3. Add $1$ in binary to get $1111111011010100$. 

Therefore $-300_{10} = 1111111011010100_2$. 

## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/583067547?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 1.9: Two's complement representation"></iframe></div>


Other resources: 
- [More examples at TutorialsPoint](https://www.tutorialspoint.com/two-s-complement)
- [YouTube video from MIT OpenCourseware with more worked examples](https://www.youtube.com/watch?v=m_G3z-C1C2g)
- [Two's complement calculator](https://www.easycalculation.com/twos-complement.php) -- only works for integers between $-128$ and $127$, and it doesn't include leading `0` bits in the answer. 

## Practice 
