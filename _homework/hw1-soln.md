---
layout: page
title: Homework 1 Solutions
permalink: /homework/hw1-soln
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* written on ancient parchement with a quill and then flown to the instructor via owl post like in Harry Potter

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:**

Answer the following problems regarding permutations in $$S_7$$.

* (a) Rewrite the following permutation as a product of disjoint cycles

$$\binom{1\ 2\ 3\ 4\ 5\ 6\ 7}{2\ 7\ 4\ 3\ 1\ 5\ 6}$$

* (b) Rewrite the same permutation from (a) as a product of transpositions

* (c) Write the following permutation in standard notation

$$(13)(245)(67)$$

* (d) Determine which permutation corresponds to the following permutation matrix

$$\left(\begin{array}{ccccccc}
 0 & 0 & 1 & 0 & 0 & 0 & 0\\
 0 & 0 & 0 & 0 & 0 & 1 & 0\\
 0 & 1 & 0 & 0 & 0 & 0 & 0\\
 1 & 0 & 0 & 0 & 0 & 0 & 0\\
 0 & 0 & 0 & 1 & 0 & 0 & 0\\
 0 & 0 & 0 & 0 & 0 & 0 & 1\\
 0 & 0 & 0 & 0 & 1 & 0 & 0\\
\end{array}\right)$$

**Solution:**

* (a) $$(12765)(34)$$
* (b) $$(12)(27)(76)(65)(34)$$
* (c) $$\binom{1\ 2\ 3\ 4\ 5\ 6\ 7}{3\ 4\ 1\ 5\ 2\ 7\ 6}$$
* (d) $$\binom{1\ 2\ 3\ 4\ 5\ 6\ 7}{4\ 3\ 1\ 5\ 7\ 2\ 6}$$

**Problem 2:** 
Let $$G$$ be a group and $$a\in G$$.
The **order** $$\lvert |a \rvert|$$ of an element $$a\in G$$ is

$$\lvert a\rvert = \min \{k: k\geq 1,\quad a^k=e\}.$$

Determine the largest possible order of an element of each of the following groups, and give an example of an element with that order.

* (a) $$\mathbb{Z}_7$$
* (b) $$\mathbb{Z}_7^\times$$
* (c) $$S_7$$

**Solution:**

* (a) The largest possible order of an element is $$7$$, and $$1$$ has this order.
* (b) The largest possible order of an element is $$6$$, and $$3$$ has this order.
* (c) The largest possible order of an element is $$12$$, and $$(123)(4567)$$ has this order.  Notice that the order of an element is the least common multiple of the lengths of its cycles, when written as a product of disjoint cycles.

**Problem 3:**

For each of the following, give an example of a group with the desired property.

* (a) a non-Abelian group whose center has only one element
* (b) a non-Abelian group whose center has exactly two elements
* (c) a group with two elements $$a,b$$ of finite order, where $$a\ast b$$ has infinite order

**Solution:**

* (a) the center of $$S_3$$ is only $$e$$
* (b) the center of $$\text{SL}_2(\mathbb{R})$$ is $$\{I,-I\}$$
* (c) take $$A,B\in\text{SL}_2(\mathbb{R})$$ with

$$
A = \frac{1}{\sqrt{2}}\left(\begin{array}{cc}1 & -1\\1 & 1\end{array}\right),\quad\text{and}\quad
B = \frac{1}{\sqrt{2}}\left(\begin{array}{cc}2 & -2\\1 & 0\end{array}\right).
$$

Then $$A^4 = I$$ and $$B^4 = I$$, so $$A$$ and $$B$$ have finite order.  However

$$AB = \left(\begin{array}{cc}1/2 & -1\\3/2 & -1\end{array}\right),$$

has infinite order.

**Problem 4:** A Mobius transformation is a function of the form

$$\chi: \mathbb C\rightarrow\mathbb C,\quad \chi(z) = \frac{az+b}{cz+d}$$

for some complex numbers $$a,b,c,d\in\mathbb{C}$$ with $$ad-bc\neq 0$$.

Prove that the set $$\mathcal M$$ of all Mobius transformations is a group with binary operation given by composition.
This group is sometimes called the Mobius group.

**Solution:**
Suppose $$\chi,\eta\in\mathcal M$$.
Then $$\chi(z) = \frac{az+b}{cz+d}$$ and $$\eta(z) = \frac{pz+q}{rz + s}$$ for some $$a,b,c,d,p,q,r,s\in\mathbb{C}$$ with  $$ad-bc\neq 0$$ and $$ps-rq\neq 0$$.
Moreover

$$\chi(\eta(z)) = \frac{a\eta(z)+b}{c\eta(z)+d} = \frac{a\frac{pz+q}{rz + s}+b}{c\frac{pz+q}{rz + s}+d} = \frac{(ap+br)z + aq+bs}{(cp+rd)z+cq+sd}.$$

Since

$$(ap+br)(cq+sd)-(aq+bs)(cp+rd) = (ad-bc)(ps-rq)\neq 0,$$

this shows that $$\chi\circ\eta\in \mathcal{M}$$.
Thus the composition of Mobious transformations is also a Mobious transformation, showing that the binary operation is well-defined.
Since composition of functions is associative, we get that the binary operation is associative automatically.

The identity function $$\iota(z) = z = \frac{1z + 0}{0z + 1}$$ is in $$\mathcal M$$, and satisfies $$\iota\circ \chi = \chi\circ\iota = \chi$$ for all $$\chi\in\mathcal M$$, so $$\iota$$ is an identity for $$\mathcal M$$.

One easily verifies that the inverse function of $$\chi(z) = \frac{az+b}{cz+d}$$ is $$\chi^{-1}(z) = \frac{dz-b}{-cz+a}$$, and since $$da-(-b)(-c)= ad-bc\neq 0$$, we have that $$\chi^{-1}(z)\in\mathcal M$$.
Since $$\chi\circ\chi^{-1} = \chi^{-1}\circ\chi = \iota$$, each element of $$\mathcal M$$ has an inverse.  Thus $$\mathcal M$$ is a group.

**Problem 5:** Suppose that $$G\subseteq \mathbb R^3$$ with the property that

$$\vec u,\vec v\in G\quad\Rightarrow\quad \vec u\times\vec v\in G,$$

where here $$\times$$ dentes the cross product.

Prove that if $$G$$ is a group under the binary operation $$\times$$, then $$G = \{\vec 0\}$$.

**Extra credit:**  Prove that if $$G$$ is a semigroup under the binary operation $$\times$$, then $$\dim\text{span}(G) \leq 1$$.

**Solution:**

Suppose that $$G$$ is a group and that $$\vec v\in G$$.
Then $$\vec v \times \vec v = \vec 0$$, and  $$\vec v\times (\vec v\times \vec v) = \vec v\times 0 = \vec 0$$.
This means

$$\vec v \times \vec v = \vec v\times (\vec v\times \vec v),$$

since both sides are equal to zero.  Since a group has inverses, we should have left cancelation so that $$\vec v = \vec v\times \vec v$$.
This proves that $$\vec v = \vec 0$$.  Since $$\vec v\in G$$ was arbitrary, this shows $$G \subseteq \langle \vec 0\rangle$$.
Since $$G$$ is a group, it must be non-empty and thus $$G = \langle\vec 0\rangle$$.

**Extra credit solution:**

The point is that the cross product of vectors is typically not associative, ie.

$$\vec u\times (\vec v\times \vec w) \neq (\vec u\times \vec v)\times \vec w,$$

unless $$\vec u$$, $$\vec v$$, and $$\vec w$$ satisfy certain pretty restrictive constraints.
However, if $$G$$ is a semigroup then the binary operation must be associative, and this imposes a restriction on all the elements in $$G$$.

Suppose that $$G$$ is a semigroup.
If $$\vec v,\vec w\in G$$, then the fact that the binary operation on $$G$$ has to be associative implies

$$(\vec v\times \vec w)\times\vec w = \vec v\times (\vec w\times \vec w) = \vec v\times \vec 0 = \vec 0.$$

By properties of the cross product, we know that $$\vec v\times \vec w$$ must be perpendicular to $$\vec w$$, and therefore

$$\lvert (\vec v\times \vec w)\times\vec w\rvert  = \lvert \vec v\times \vec w\rvert \cdot \lvert \vec w\rvert.$$

Since $$(\vec v\times \vec w)\times\vec w = \vec 0$$, this shows that

$$\lvert \vec v\times \vec w\rvert \cdot \lvert \vec w\rvert = 0,$$

and therefore either $$\vec v\times \vec w = \vec 0$$ or else $$\vec w = \vec 0$$, in which case $$\vec v\times \vec w = \vec 0$$ anyway.
The cross product is zero exactly when the vectors are parallel, and since $$\vec v$$ and $$\vec w$$ were arbitrary, this proves that every two vectors in $$\vec v$$ are parallel. 
Thus either $$G = \{\vec 0\}$$ and $$\dim(G) = 0$$, or $$G \subseteq \text{span}(\{\vec v\})$$ for some nonzero vector $$\vec v\in G$$ and 

$$\dim\text{span}(G) = \dim\text{span}(\{\vec v\}) = 1.$$








