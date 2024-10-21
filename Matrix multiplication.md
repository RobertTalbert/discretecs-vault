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

Notes: 
* Matrix multiplication is *not* simply multiplying the corresponding entries of the two matrices together. 
* The product of $A$ and $B$ is only defined if the number of columns in $A$ equals the number of rows in $B$. Otherwise $AB$ cannot be computed. For example if $A$ is a $3 \times 4$ matrix and $B$ is $4 \times 7$, then $AB$ can be computed, and the result will be a $3 \times 7$ matrix. But note, $BA$ cannot be computed because the number of columns in $B$ (7) does not equal the number of rows in $A$ (3). 
* The previous point illustrates that multiplication of matrices does 
* Using the language of vectors, the $(i,j)$-entry of $AB$ is the [dot product](https://www.mathsisfun.com/algebra/vectors-dot-product.html) of the $i$th column of $A$ with the $j$th column of $B$. 

## Examples and Non-Examples

## Resources 

(video)

Other resources: 
- 

## Practice 
