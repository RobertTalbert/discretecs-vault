---
aliases: [functions, function]
--- 

#sets-functions 

## Definition 

> [!tldr] Definition
> A **function** is a rule that accepts input from one [[Set|set]] and produces output in another set, so that every input is assigned to one and only one output. If the inputs come from from the set $A$ and the outputs come from the set $B$, and the name of the function is $f$, then we write $f: A \rightarrow B$. 

Notes: 
- In the notation above ($f: A \rightarrow B$) the set $A$ is the [[Domain|domain]] of the function and the set $B$ is the [[Codomain]]. 
- If $x \in A$, then the output that is assigned to $x$ by the function $f$ is notated $f(x)$ ("f of x"). This is sometimes called the *image* of $x$.
- Functions can take on different forms or representations. Common forms are: 
	- *Formulas*. For example $f: \mathbb{Z} \rightarrow \mathbb{Z}$ defined by $f(n) = 2n$ is a function that assigns each [[Integers|integer]] input $n$ to its double. 
	- *Tables or lists*. For example $g: \{0,1,2\} \rightarrow \{a,b,c\}$ defined by $g(0) = c$, $g(1) = a$, $g(2) = b$ is a function, defined by explicitly listing the outputs assigned to each input. 
	- *Verbal descriptions.* For example, define the function $p: \mathbb{N} \rightarrow \mathbb{N}$ by assigning $n$ to the $n$th digit of $\pi$. So $p(0) = 3$, $p(1) = 1$, $p(2) = 4$, $p(3) = 1$, etc. 
	- *Graphs or diagrams*. For example the diagram below defines a function from $A = \{-2,0,3,5\}$ to $B = \{-4,-3,4\}$: 
![[simple-function-diagram.png|300]]
([Source](https://mathbooks.unl.edu/PreCalculus/Intro-to-Functions.html))

- In order for a rule of assignment to be a valid function according to this definition, two things must happen: 
	- Every point in $A$ (the [[Domain|domain]] of $f$) must actually have an output; that is, there can be no [[Set|elements]] of $A$ that are unassigned or uncomputable. 
	- No point in $A$ can be sent to two different outputs. 
- However notice in the examples above, and below, that **it is within the definition for two different inputs to be sent to the same output** (a "collision"). We just cannot send *one* input to *two or more* outputs ("splitting").

## Examples and Non-Examples

Some examples are shown above; here are a few more. 

- The function $ceil: \mathbb{R} \rightarrow \mathbb{Z}$ takes a real number (floating point number) as input, and the output assigned is the integer you get when you round the input up. For example $ceil(9.22) = 10$. This is a function because every input does receive an output, and no input gets more than one. (However there are lots of collisions, where different inputs are sent to the same output; for example every number greater than 9 and less than or equal to 10 will be sent to 10.)
- The function $f: \mathbb{R} \rightarrow \mathbb{R}$ defined as the formula $f(x) = x^2$ is a function, since every number can be squared and no number has more than one square. (Again however there are collisions, since $f(1) = f(-1)$.)

Some examples of assignments or mappings that are *not* functions: 
- The mapping $g: \mathbb{R} \rightarrow \mathbb{R}$ given by $g(x) = \sqrt{x}$ is not a valid function because some inputs do not have outputs, for example $x=-1$. This number does not have an "output" because $g(-1)$ is not a real number; it has nothing to which it is assigned in the [[Codomain|codomain]]. 
- The mapping  $h: \{0,1,2\} \rightarrow \{a,b,c\}$ defined by $h(0) = p$, $h(1) = a$, $h(2) = b$ is not a function because the output for $0$ does not exist in the set $\{a,b,c\}$. 
- The mapping $k: \{0,1,2\} \rightarrow \{a,b,c\}$ defined by $k(0) = a$, $k(1) = b$, $k(2) = c$, $k(1) = a$ is not a function because the input $1$ is assigned to two different outputs. 
- The mapping that matches each person to their phone number is not a function, because some people have more than one phone number, causing some inputs to "split" into different outputs. 

## Resources 

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/614432178?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Screencast 3.8: Functions"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

