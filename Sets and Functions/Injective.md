---
aliases: [injective, injection, one-to-one]
--- 

#sets-functions 

## Definition 

> [!tldr] Definition
> A [[Function|function]] $f: A \rightarrow B$ is **injective** if, for all pairs of inputs $a_1, a_2 \in A$, if $a_1 \neq a_2$ then $f(a_1) \neq f(a_2)$. 

**Notes:**
- An informal English way of describing injective functions is: If two inputs are different, then their outputs are different if the function is injective. 
- In other words there are no "collisions" where different inputs are mapped to the same output. 
- An equivalent way to define an injective function is to use the [[Contrapositive|contrapositive]] of the [[Conditional statements|conditional statement]] in the above definition: The function $f: A \rightarrow B$ is injective if, for all $a_1, a_2 \in A$, if $f(a_1) = f(a_2)$ then $a_1 = a_2$. 
- Injective functions are often referred to as *one-to-one*.  

> [!danger] One-to-one does not mean "every input goes to exactly one output"
> 
> The phrase "one-to-one" does *not* mean that "every input goes to exactly one output". Having each input go to exactly one output is a property that *all* functions have, including those that are not injective. Injective functions are "one-to-one" as opposed to "two-to-one", where two different inputs map to the same output. This potential confusion is why "injective" is a better word to use than "one-to-one"; avoid using the latter. 

## Examples and Non-Examples

- The function $f: A \rightarrow B$ shown in the diagram below is injective, because there are no collisions -- whenever the inputs are different, the outputs are different. 

![[injective1.png|300]]
([Image source](https://www.google.com/url?sa=i&url=https%3A%2F%2Fcollegedunia.com%2Fexams%2Fbijective-function-mathematics-articleid-5395&psig=AOvVaw3bIRWsNf8Mn9zace0S4B8A&ust=1696082301870000&source=images&cd=vfe&opi=89978449&ved=0CBIQjhxqFwoTCLj4zor9z4EDFQAAAAAdAAAAABAE))

- The function that takes the names of students at a university as input, then returns their student ID numbers as output, is (we hope) injective, because no two different students should have the same ID number. 
- The function $g: \mathbb{N} \rightarrow \mathbb{Z}$ defined by the formula $g(n) = 2n$ is injective, because if $a_1 \neq a_2$, then $2a_1 \neq 2a_2$. 

Here are some non-examples: 
- The function in the diagram below is *not* injective, because $3$ and $4$ are different but are mapped to the same point in the [[Codomain|codomain]], namely $C$. It's a "collision". 
![[non-injective.png]]
- The function that takes the names of students at a university as input, then returns their initials as output, is not injective since two different students with the same initials would be mapped to the same output. 
- The function $h: \mathbb{N} \rightarrow \mathbb{Z}$ defined by the formula $h(n) = n^2 - 2n$ is not injective, since $h(0) = 0$ but also $h(2) = 0$. 

## Resources 

<iframe src="https://player.vimeo.com/video/614452153?h=58ba81862d" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/614452153">Screencast 3.9: Injective functions</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

Other resources: 
- An older video for MTH 210 (Communicating in Mathematics): 
<iframe width="560" height="315" src="https://www.youtube.com/embed/fGYaaKryZp4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

- Tutorial: [Injective functions](https://byjus.com/maths/one-to-one-function)
