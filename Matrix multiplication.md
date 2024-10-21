---
aliases:
  - matrix multiplication
tags:
  - basic-concepts
created: 2024-10-21
updated:
---
---
## Definition 

> [!tldr] Definition
> Let $A$ be an $m \times k$ [[Matrix|matrix]] (that is, a matrix with $m$ rows and $k$ columns) and let $B$ be a $k \times n$ matrix ($k$ rows, $n$ columns). Then the **product** of $A$ and $B$, denoted by $AB$, is the $m \times n$ matrix whose $(i,j)$-entry is the sum of the products of the elements in the $i$th row of $A$ and the $j$th column of $B$. That is, if $c_{ij}$ is the $(i,j)$-entry then 
> $$c_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j} + \cdots + a_{ik}b_{kj}$$

**Notes**: 
* Matrix multiplication is *not* simply multiplying the corresponding entries of the two matrices together. 
* The product of $A$ and $B$ is only defined if the number of columns in $A$ equals the number of rows in $B$. Otherwise $AB$ cannot be computed. For example if $A$ is a $3 \times 4$ matrix and $B$ is $4 \times 7$, then $AB$ can be computed, and the result will be a $3 \times 7$ matrix. But note, $BA$ cannot be computed because the number of columns in $B$ (7) does not equal the number of rows in $A$ (3). 
* The previous point illustrates that multiplication of matrices does not obey the [[Properties of arithmetic|commutative property]]: It is not necessarily true that for any two matrices $A$ and $B$ that $AB = BA$. In fact $BA$ may not even be computable, even if $AB$ is. 
* Using the language of vectors, the $(i,j)$-entry of $AB$ is the [dot product](https://www.mathsisfun.com/algebra/vectors-dot-product.html) of the $i$th column of $A$ with the $j$th column of $B$. 
* If $A$ is a square matrix -- that is, it has the same number of rows as columns -- then we can multiply it to itself. Doing so creates a **power** of a matrix: $AA = A^2$. If $A$ is $n \times n$, then so is $A^2$. Therefore we can also compute the third power, $A^3$, which would be defined as $A^3 = A \times A^2$. In general, the $k$th power of a square matrix is defined [[Recursion|recursively]]: $A^2 = AA$ and then for any $k > 2$, $A^k = A A^{k-1}$. 

## Examples 

Let $A$ and $B$ be the following matrices: 
$$A = \begin{bmatrix} 1 & 0 & 4 \\ 2 & 1 & 1 \\ 3 & 1 & 0 \\ 0 & 2 & 2 \end{bmatrix} \qquad 
B = \begin{bmatrix} 2 & 4 \\ 1 & 1 \\ 3 & 0  \end{bmatrix}$$
Notice that $A$ is $4 \times 3$ and $B$ is $3 \times 2$. Since the number of columns of $A$ matches the number of rows in $B$, we can compute the product $AB$ (but not the product $BA$). The result will be a $4 \times 2$ matrix. The $(1,1)$-entry of $AB$ is the sum of the products of elements in the first row of $A$ with the first column of $B$: 
$$(1)(2) + (0)(1) + (4)(3) = 14$$
The $(1,2)$-entry is the sum of the products of the elements of the first row of $A$ with the second column of $B$: 
$$(1)(4) + (0)(1) + (4)(0) = 4$$
The $(2,1)$-entry is the sum of the products of the elements of the second row of $A$ with the first column of $B$: 
$$(2)(2) + (1)(1) + (1)(3) = 8$$
The $(2,2)$-entry is the sum of the products of the elements of the second row of $A$ with the second column of $B$: 
$$(2)(4) + (1)(1) + (1)(0) = 9$$
Continuing this process leads to the following result: 
$$\begin{bmatrix} 14 & 4 \\ 8 & 9 \\ 7 & 13 \\ 8 & 2 \end{bmatrix}$$


**Powers of a matrix:** Consider the following $3 \times 3$ matrix $A$ whose entries are either 0 or 1.
$$A = \begin{bmatrix} 0 & 1 & 1 \\ 1 & 0 & 0 \\ 1 & 1 & 1 \end{bmatrix}$$
Since $A$ is square, we can find $A^2$ which is the product of $A$ with itself: 
$$A^2 = \begin{bmatrix} 0 & 1 & 1 \\ 1 & 0 & 0 \\ 1 & 1 & 1 \end{bmatrix} \begin{bmatrix} 0 & 1 & 1 \\ 1 & 0 & 0 \\ 1 & 1 & 1 \end{bmatrix}$$
This equals: 
$$\begin{bmatrix} (0)(0) + (1)(1) + (1)(1) & (0)(1)+(1)(0)+(1)(1) & (0)(1)+(1)(0)+(1)(1) \\ (1)(0) + (0)(1) + (0)(1) & (1)(1)+(0)(0)+(0)(1) & (1)(1)+(0)(0)+(0)(1) \\
(1)(0) + (1)(1) + (1)(1) & (1)(1)+(1)(0)+(1)(1) & (1)(1)+(1)(0)+(1)(1)\end{bmatrix} 
= \begin{bmatrix} 2 & 1 & 1 \\ 0 & 1 & 1 \\ 2 & 2 & 2 \end{bmatrix} $$
Likewise, 
$$A^3 = A \cdot A^2 = \begin{bmatrix} 0 & 1 & 1 \\ 1 & 0 & 0 \\ 1 & 1 & 1 \end{bmatrix} \begin{bmatrix} 2 & 1 & 1 \\ 0 & 1 & 1 \\ 2 & 2 & 2 \end{bmatrix} = 
\begin{bmatrix} 2 & 3 & 3 \\ 2 & 1 & 1 \\ 4 & 4 & 4 \end{bmatrix}$$

## Resources 

(video)

Other resources: 
- 

## Practice 
