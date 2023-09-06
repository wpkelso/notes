---
tags:
  - mathematics
  - programming
  - data_structures
  - logic
  - discrete_mathematics
---
# Set

## Mathematics 

In mathematics, a set is a collection of any numbers of–including none–objects (numbers, other sets, etc.) that are related, and considered as a single object. The only thing that matters in relation to a set is what the elements in the set are, not how the set is specified, how the elements are ordered, or how many times the elements in the set are counted.

### Properties & Related Theories

#### Extensionality

> [!note] Definition
> If $A$ and $B$ are sets, then $A=B$ iff every element of $A$ is also an element of $B$, and vice versa

This allows a way of showing that sets are identical (i.e. $A\equiv B$).

#### Subsets

> [!note] Definition
> If every element of $A$ is also an element of $B$, then $A$ can be considered a *subset* of $B$ and can be written as $A \subseteq B$. If $A \subseteq B$ but $A \neq B$, then $A$ is a *proper subset* of $B$.

This definition allows extrapolation to say that if $A \subseteq B$ and $B \subseteq A$ then $A=B$.

#### Power Sets

>[!note] Definition
>The set $\mathcal{P}(A)$ consisting of all subsets of the set $A$ $$\mathcal{P}(A)={B:B\subseteq A}$$

It should be noted that due to the definition of power sets and subsets, it naturally follows that $\mathcal{P}(\emptyset)=\{ \emptyset  \}$.

### Important Sets

- $\mathbb{N}=\{ 0,1,2,3,\dots \}$ is the set of natural numbers 
- $\mathbb{Z}=\{ \dots,-2,-1,0,1,2,\dots \}$ is the set of integers
- $\mathbb{Q}=\{ \frac{m}{n}:m,n\in \mathbb{Z}\:\text{and}\:n \neq 0\}$ is the set of rational numbers
- $\mathbb{R}=(-\infty,\infty)$ is the set of all real numbers
- $\emptyset = \{  \}$ is a set containing no elements, and is a subset of **every** set
## Programming
Similarly to in mathematics, a set in programming is an [[Abstract Data Type|abstract data type]] representing a group of objects in which order doesn’t matter but duplicate items are **not** allowed. They will often be implemented with a [[Binary Search Tree|BST]] or a [[Hash Table|hash map]].
