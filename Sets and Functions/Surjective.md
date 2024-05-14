---
aliases: [surjective, surjection, onto]
--- 

#sets-functions 

## Definition 

> [!tldr] Definition
> A [[Function|function]] $f: A \rightarrow B$ is **surjective** if, for every point $b \in B$, there exists at least one point $a \in A$ such that $f(a) = b$. 

**Notes:**
- An informal English way of describing surjective functions is: Each point in the [[Codomain|codomain]] is "covered" or "hit" by at least one point in the [[Domain|domain]]. 
- In other words there are no points in the codomain that are "left out" by the mapping. 
- Surjective functions are often referred to as *onto*. 
- If $f$ is surjective, then the codomain of $f$ and the [[Range|range]] of $f$ are the same. (The [[Converse|converse]] of that statement is also true -- if a function $f$ has equal codomain and range, then $f$ is surjective.)

## Examples and Non-Examples

- The function $f: A \rightarrow B$ shown in the diagram below is surjective, because each of the four points in the codomain $B$ has at least one point in $A$ mapping to it. 

![[injective1.png|300]]
([Image source](https://www.google.com/url?sa=i&url=https%3A%2F%2Fcollegedunia.com%2Fexams%2Fbijective-function-mathematics-articleid-5395&psig=AOvVaw3bIRWsNf8Mn9zace0S4B8A&ust=1696082301870000&source=images&cd=vfe&opi=89978449&ved=0CBIQjhxqFwoTCLj4zor9z4EDFQAAAAAdAAAAABAE))

- The function below is surjective because every point in the codomain has at least one point mapping onto it. However the function is not [[Injective|injective]] because there one of the points in $B$ has multiple domain elements mapping to it. 
![[surj-not-inj.png|150]]
- The function $g: \mathbb{Z} \rightarrow \mathbb{Z}$ defined by the formula $g(n) = n+3$ is surjective, because every point in the codomain, which is the set of all integers, has at least one point in the domain that maps on to it. Namely, if $b$ is any point in the codomain then $b-3$ in the domain maps on to $b$, since $g(b-3) = (b-3) + 3 = b$. This mapping is also [[Injective|injective]]. 

Here are some non-examples: 
- The function below is *not* surjective because the points $2$ and $7$ in the codomain (the set on the right) do not have anything mapping to them. (This function *is* [[Injective|injective]], however.)
![[not-surj.png|300]]
- Consider the function from the set of all current students at your university, to the set of all seven-digit integers, where each student is mapped to their primary phone number (without the area code). This function is highly unlikely to be surjective, as there are certain seven-digit numbers that would never be assigned as someone's phone number, like 000-0000. 
- The function $h: \mathbb{N} \rightarrow \mathbb{Z}$ defined by the formula $h(n) = 2n$ is not surjective, since there are points in the codomain ($\mathbb{Z}$, the set of all integers) with nothing mapping on to them. For example there is no natural number that maps on to $3$ (the only number that would map to $3$ with this function is $3/2$ which is not an element of $\mathbb{N}$); and there is nothing in $\mathbb{N}$ that maps on to $-4$. 
- The function $g: \mathbb{N} \rightarrow \mathbb{Z}$ defined by the formula $g(n) = n+3$ is **not** surjective, because nothing in $\mathbb{N}$ would map onto the point $-2$ in the codomain. The number that would "work" is $-5$ but that's not in the domain. Notice, this is the same *formula* as given above for an example of a function that *is* surjective, but it's a different *function* because the domain is now different. 

> [!danger] The domain and codomain matter 
> As the last examples point out, the same rule of assignment might result in a surjective function in one situation but a non-surjective function in others if the domains and codomains are different. So, a function is not 100% determined by its formula or rule of assignment -- the domain and codomain are also essential. 



## Resources 
<iframe src="https://player.vimeo.com/video/614525515?h=065c033a89" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/614525515">Screencast 3.10: Surjective functions</a> from <a href="https://vimeo.com/user132700952">Robert Talbert</a> on <a href="https://vimeo.com">Vimeo</a>.</p>


Other resources: 
- An older video from MTH 210 (Communicating in Mathematics): 
<iframe width="560" height="315" src="https://www.youtube.com/embed/jVniPMIexQE?si=eJwmGV8-iwAr8gVL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
