---
aliases: [base conversion algorithm]
--- 

#computer-arithmetic 

## Process 

> [!tldr] To convert a positive [[Integers|integer]] *from* [[Base 10 representation|base 10]] *to* base $b$ where $b$ is any other number base: 
> Let $n$ be the integer in base 10 that you want to convert to base $b$. 
> 1. Divide $n$ by $b$. Let $q_1$ be the quotient (how many times $b$ goes into $n$) and let $r_1$ be the remainder. 
> 2. Now replace $n$ with $q_1$. Divide $q_1$ by $b$, and let $q_2$ be the new quotient and $r_2$ be the new remainder. 
> 3. Replace $q_1$ with $q_2$. Divide $q_2$ by $b$, and let $q_3$ be the new quotient and $r_3$ be the new remainder. 
> 4. Continue these steps (divide the previous quotient by $b$ and keeping the new quotient and new remainder) until the new quotient is $0$. In the final step where the new quotient is $0$, go ahead and keep the. new remainder (which will just be the number you divided into). 
> 5. The base $b$ representation of the original integer $n$, is **the sequence of remainders written in reverse order**. So, if there were $k$ steps in all, the base $b$ representation is $r_k r_{k-1} r_{k-2} \cdots r_3 r_2 r_1$. 

Notes: 
- The algorithm here always terminates because the quotients are [[Natural numbers|nonnegative integers]], and at each step must get strictly smaller, and therefore they will always converge to zero. 
- Here is Python code for this algorithm if the base is between 2 and 10. It terminates immediately if the base is larger than 10, because to convert to a larger base you would need alphabetical replacements for the numbers 10 and above, as in [[Base 16 representation|hexadecimal]]. You could modify this code, though, to work for larger bases if you introduced some additional data structures to represent 10, 11, 12, etc. Also, notice this returns a string, not a number. 

```python
def convert_to_base(number, base):

  if base < 2 or base > 10:
    raise ValueError("Invalid base: %d" % base)

  digits = []
  while number:   # Loop exists once "number" equals 0
    digit = number % base #Divide by the base and keep the remainder
    digits.append(chr(ord('0') + digit)) 
    number //= base # Replace "number" with the previous quotient 

  digits.reverse()
  return ''.join(digits)
```

## Examples

Converting the base 10 integer $42$ to [[Base 2 representation|binary]] ([[Base 2 representation|base 2]]): 

1. Divide $42$ by $2$ and keep the quotient and remainder: $q_1 = 21, r_1 = 0$
2. Divide $q_1$ by $2$ and keep the quotient and remainder: $q_2 = 10, r_2 = 1$
3. Divide $q_2$ by $2$ and keep the quotient and remainder: $q_3 = 5, r_3 = 0$
4. Divide $q_3$ by $2$ and keep the quotient and remainder: $q_4 = 2, r_4 = 1$
5. Divide $q_4$ by $2$ and keep the quotient and remainder: $q_5 = 1, r_1 = 0$
6. Divide $q_5$ by $2$ and keep the quotient and remainder: $q_6 = 0, r_1 = 1$. This is because $2$ goes into $1$ zero times, with a remainder of $1$. 
7. The quotient equalled zero, so stop and return the remainders in reverse order: $101010$. That is, $42_{10} = 101010_2$. 

Convert the [[Base 10 representation|base 10]] integer 42 to base $9$: 
1. Divide $42$ by $9$ and keep the quotient and remainder: $q_1 = 4, r_1 = 6$
2. Divide $4$ by $9$ and keep the quotient and remainder: $q_2 = 0, r_2 = 4$
3. The quotient equalled zero, so stop and return the remainders in reverse order: $46$. That is, $42_{10} = 46_9$. 

Convert the base 10 integer 420 to [[Base 16 representation|hexadecimal]] (base 16): 
1. Divide $420$ by $16$ and keep the quotient and remainder: $q_1 = 26, r_1 = 4$
2. Divide $26$ by $16$ and keep the quotient and remainder: $q_2 = 1, r_2= 10$
3. Divide $1$ by $16$ and keep the quotient and remainder:  $q_3 = 0, r_3 = 1$
4. The quotient equalled zero, so stop and return the remainders in reverse order. But notice we can't use "10" as one of the remainders because it would be ambiguous (is it 10, or a 1 in one place and a 0 in another?). So we have to convert $10$ to $A$ in base 16 first. Having done that, the [[base 16 representation]] is $1A4$. That is, $420_{10} = 1A4_{16}$. 
## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/578187581?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 1.3: Base 10 conversion algorithm"></iframe></div>


Other resources: 
- [More examples at TutorialsPoint](https://www.tutorialspoint.com/computer_logical_organization/number_system_conversion.htm)
- [Trinity College textbook section on this algorithm](http://turing.cs.trincoll.edu/~ram/cpsc110/inclass/conversions.html)

## Practice 
To practice this concept: 
- Generate a random integer in base 10 and a random base (or use one of our standard bases: $2$, $8$, or $16$). 
- Follow the algorithm to convert from [[Base 10 representation|base 10]] to your chosen base. 
- Check your work using the Python code above, or one of the base conversion calculators found [here](https://www.rapidtables.com/convert/number/index.html). 