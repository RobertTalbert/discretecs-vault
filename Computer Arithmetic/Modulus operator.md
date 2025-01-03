---
aliases: [modulus, modulus operator, mod, the Modulus operator, the modulus operator]
--- 

#computer-arithmetic 

## Definition 

> [!tldr] Definition
> The **modulus operator** `%` when applied to two integers $a$ and $b$, returns the unique value of the remainder $r$ given by the [[Division algorithm|Division Algorithm]] when dividing $a$ by $b$. 

Notes:
- The symbol `%` is used in Python and many other languages to implement the modulus operator. 
- According to the [[Division algorithm|Division Algorithm]], the result of `a % b` is always strictly less than $b$. 
- If $b = 0$ then `a % b` is undefined (and will throw an error in Python). 
- `a % b` can be found if $a$ is negative as well; see below for the procedure. 
- You can find `a % b` using just a Google search page. For example open up a Chrome browser tab and enter `100 % 8` in the URL field and see what happens. 

## Examples and Non-Examples

- `100 % 8 = 4` because $8$ divides $100$, $12$ times with a remainder of $4$. 
- `100 % 5 = 0` because $5$ evenly divides $100$. 
- `225225 % 14 = 9`
 

> [!NOTE] To find `a % b` if $a$ is negative: 
> Add $b$ to $a$ repeatedly until the result is non-negative (zero or higher). When this happens, the result is `a % b`. 
> 
> Example: To find `(-100) % 16`, start adding $16$ to $-100$ and stop when you hit zero or a positive result: 
> - $-100 + 16 = -84$
> - $-84 + 16 = -68$
> - $-68 + 16 = -52$
> - $-52 + 16 = -36$
> - $-36 + 16 = -20$
> - $-20 + 16 = -4$
> - $-4 + 16 = 12$  STOP 
> Therefore `(-100) % 16 = 12`. (There are other ways to do this as well!)


## Resources 

The last 3 minutes of this video give more on the modulus operator: 
<iframe src="https://player.vimeo.com/video/583046507?h=ef4d7d314f" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/583046507">Screencast 1.8: The Division Algorithm and the modulus operator</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- [How to use the mod operator in Python](https://realpython.com/python-modulo-operator/)

## Practice 

To practice finding `a % b` by hand, simply generate a random pair of integers and see if you can compute the result by hand; then check work using Python or some other computing resource. 