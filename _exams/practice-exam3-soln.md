---
layout: page
title: Practice Exam 3 Solutions
permalink: /exams/practice-exam3-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

Unless otherwise stated, all rings will be commutative with identity and all ring homomorphisms will send the identity to the identity.

## Problem 1 (True or False)

* (a) The element $$\sqrt{\pi}$$ is algebraic over $$\mathbb Q(\pi)$$
* (b) The field extension $$\mathbb Q(\sqrt{2},\sqrt{3})$$ is simple
* (c) If $$I$$ is a radical ideal of $$R$$, then $$R/I$$ is a reduced ring
* (d) Every Euclidean domain is a principal ideal domain
* (e) Greatest common divisors, when they exist, are unique

**Solution:**
T,T,T,T,F

## Problem 2

* (a) State the definition of an ideal $$I$$ in a ring $$R$$
* (b) Prove that if $$I,J\subseteq R$$ are ideals, then $$I\cap J$$ is an ideal
* (c) Prove that if $$I,J\subseteq R$$ are ideals, then

$$IJ = \{a_1b_1+a_2b_2+\dots + a_nb_n: a_j\in I,\ b_j\in J\}$$

is also an ideal.
* (d) Prove that $$IJ\subseteq I\cap J$$
* (e) Give an example where $$IJ\neq I\cap J$$

**Solution:**

* (a) An ideal $$I$$ is an additive subgroup of $$R$$ with the property that if $$a\in R$$ and $$b\in I$$ then $$ab\in I$$
* (b) Intersections of subgroups are subgroups, so $$I\cap J$$ is an additive subgroup.  If $$a\in R$$ and $$b\in I\cap J$$, then $$b\in I$$ so $$ab\in I$$ and $$b\in J$$ so $$ab\in J$$, and therefore $$ab\in I\cap J$$.  Thus $$I\cap J$$ is an ideal.
* (c) It is clearly an additive subgroup.  Furthermore, if $$a_1,\dots, a_n\in I$$ and $$b_1,\dots, b_n\in J$$ then and $$c\in R$$, then for all $$j$$ we have $$ca_j\in I$$ and therefore by definition
$$c(a_1b_1+a_2b_2+\dots+a_nb_n)=(ca_1)b_1+(ca_2)b_2+\dots+(ca_n)b_n\in IJ.$$
This shows $$IJ$$ is an ideal.
* (d) If $$a_1,\dots, a_n\in I$$ and $$b_1,\dots, b_n\in J$$ then for all $$j$$ we have $$a_jb_j\in I$$ and $$a_jb_j\in J$$ so that $$a_jb_j\in I\cap J$$.  It follows that the combination $$a_1b_1+a_2b_2+\dots+a_nb_n\in I\cap J$$.  Hence $$IJ\subseteq I\cap J$$.
* (e) As an example, take $$I = J = (2)\in \mathbb{Z}$$.  Then $$I\cap J=(2)$$ but $$IJ = (4)$$.

## Problem 3

* (a) Write down the definition of a principal ideal
* (b) Prove that if $$a,b\in R$$ are associates, then $$(a) = (b)$$
* (c) Show that the following ideal of $$\mathbb Z$$ is principal and find (with proof) a generator

$$I = \{6x+10y: x,y\in\mathbb Z\}.$$

**Solution:**

* (a) An ideal $$I\subseteq R$$ is principal if $$I = (a)$$ for some $$a\in R$$.
* (b) Suppose that $$a,b\in R$$ are associates.  Then there exists a unit $$u\in R$$ with $$a = ub$$.
Suppose $$c\in (a)$$. Then $$c = ra$$ for some $$r\in R$$.  Therefore $$c = r(ub) = (ru)b\in (b)$$.
This shows that $$(a)\subseteq (b)$$.

Conversely, suppose that $$c\in (b)$$.  Then $$c = sb$$ for some $$s\in R$$.  Therefore

$$c = sb = (su^{-1})(ub) = (su^{-1})a\in (a).$$

We conclude that $$(b)\subseteq (a)$$.  Hence $$(a) = (b)$$.

* (c) We claim that $$I = (2)$$.  Clearly everything in $$I$$ is even, so $$I\subseteq (2)$$.  Conversely, if $$a\in (2)$$ then $$a = 2k$$ for some $$k\in \mathbb{Z}$$.  Therefore

$$a = 2k = (2\cdot 6-10)k = 6(2k) + 10(-k)\in I.$$

Since $$a$$ was arbitrary, this proves that $$(2)\subseteq I$$ and therefore $$I = (2)$$.

## Problem 4

* (a) State the definition of a principal ideal domain (PID)
* (b) Prove that if $$I\subsetneq Q[x]$$ is an ideal and $$f(x)\in I$$ is irreducible, then $$I = (f(x))$$.
* (c) Let $$a = e^{2\pi i/8}$$ and suppose

$$I = \{f(x)\in\mathbb Q[x]: f(a) = 0\}.$$

Find a polynomial which generates $$I$$ as a principal ideal.

**Solution:**
* (a) A PID is an integral domain where every ideal is principal.  
* (b) Suppose that $$I\subsetneq Q[x]$$ and $$f(x)\in I$$.  Since $$I$$ is principal, there exists $$g(x)\in\mathbb Q[x]$$ with $$I = (g(x))$$.
Then since $$f(x)\in I$$, we know that

$$f(x) = h(x)g(x)$$

for some polynomial $$h(x)\in Q[x]$$.
Since $$f(x)$$ is irreducible, it follows that either $$g(x)$$ or $$h(x)$$ is a unit.
Since $$I\neq Q[x]$$, we know that $$g(x)$$ is not a unit.
Therefore $$h(x)$$ must be a unit.
This means that $$f(x)$$ and $$g(x)$$ are associates and by the previous problem it follows that $$(f(x)) = (g(x)) = I$$.

* (c) We know that $$a$$ is a root of $$x^8-1$$.  Therefore the minimal polynomial of $$a$$ divides $$x^8-1$$.  We decompose $$x^8-1$$ into irreducible factors as

$$x^8-1 = (x-1)(x+1)(x^2+1)(x^4+1).$$

The only one that has $$a$$ as a root is $$x^4+1$$, so that must be the minimal polynomial of $$a$$.
Since $$x^4+1\in I$$ and $$x^4+1$$ is irreducible, part (b) tells us that $$x^4+1$$ generates $$I$$ as a principal ideal.

## Problem 5

* (a) Write down the definition of a prime ideal
* (b) Prove that if $$I$$ is a prime ideal of a ring $$R$$, then $$R/I$$ is an integral domain.

**Solution:**

* (a) An ideal $$I$$ is prime if $$ab\in I$$ implies $$a\in I$$ or $$b\in I$$ for all $$a,b\in R$$.
* (b) Suppose that $$I$$ is prime, and let $$a,b\in R$$.  We will show that $$R/I$$ is an integral domain.
Assume that $$a+I$$ is a zero divisor.  Then $$a+I\neq 0+I$$ and there exists a nonzero $$b+I\in R/I$$ with $$(a+I)(b+I) = 0+I$$.
Therefore $$ab+I = 0+I$$, meaning that $$ab=0$$ modulo $$I$$.
This means that $$ab\in I$$ and therefore either $$a\in I$$ or $$b\in I$$.
Since $$b+I\neq 0+I$$, we know that $$b\notin I$$.
Thus we must have $$a\in I$$, meaning that $$a+I = 0+I$$, contradicting the assumption that $$a+I$$ is a zero divisor.
Thus no zero divisors exist, showing that $$R/I$$ is an integral domain.

## Problem 6

Prove that $$\mathbb Q(3 + i) = \mathbb Q(1 - i)$$.

**Solution:**

Since $$1-i = 4-(3+i)\in \mathbb Q(3+i)$$ and $$\mathbb Q\subseteq Q(3+i)$$, we know that $$\mathbb Q(1-i)\subseteq \mathbb Q(3+i)$$.
Then since $$3+i = 4-(1-i)\in \mathbb Q(1-i)$$ and $$\mathbb Q\subseteq Q(1-i)$$, we know that $$\mathbb Q(3+i)\subseteq \mathbb Q(1-i)$$.
Hence they are equal.


## Problem 7

Consider the following field extensions of $$\mathbb{Q}$$:

$$K = \mathbb Q(\sqrt{5}),\quad E = \mathbb{Q}(\sqrt{3}+\sqrt{5}).$$ 

* (a) Find a basis for $$K$$ over $$\mathbb{Q}$$
* (b) Find a basis for $$E$$ over $$\mathbb{Q}$$
* (c) Find a basis for $$E$$ over $$\mathbb{K}$$

**Solution:**

* (a) This is a simple extension by an algebraic element with minimal polynomial $$x^2-5$$, so a basis is $$\{1,\sqrt{5}\}$$
* (c) First note that the field $$E$$ is a field extension of $$K$$.  To see this, not that $$(\sqrt{3}+\sqrt{5})^2 = 8 + 2\sqrt{15}\in E$$ and therefore $$\sqrt{15}\in E$$.
Thus $$\sqrt{15}(\sqrt{3}+\sqrt{5}) = 3\sqrt{5} + 5\sqrt{3}\in E$$.
It follows that

$$3\sqrt{5}+5\sqrt{3}-5(\sqrt{3}+\sqrt{5}) = -2\sqrt{5}\in E$$

and therefore $$\sqrt{5}\in E$$. Since $$\mathbb Q\subseteq E$$, we conclude that $$K = \mathbb Q(\sqrt{5})\subseteq E$$.

Next note that $$E = K(\sqrt{3})$$.  To see this, note that 

$$3\sqrt{5}+5\sqrt{3}-3(\sqrt{3}+\sqrt{5}) = 2\sqrt{3}\in E$$

and therefore $$\sqrt{3}\in E$$.  Therefore since $$K\subseteq E$$ we have $$K(\sqrt{3})\subseteq E$$.
Conversely, $$K(\sqrt{3})$$ contains $$\sqrt{3}$$ and $$\sqrt{5}$$ and thus contains $$\sqrt{3}+\sqrt{5}$$.
Likewise it contains $$\mathbb Q$$, so $$K(\sqrt{3})$$ contains $$\mathbb Q(\sqrt{3}+\sqrt{5})$$.  Hence they are equal.

Finally it's a simple algebraic extension of $$K$$ with minimal polynomial $$x^2-3$$, so a basis is $$\{1,\sqrt{3}\}$$.

* (b) Since a basis for $$E$$ over $$K$$ is $$\{1,\sqrt{3}\}$$ and a basis for $$K$$ over $$\mathbb Q$$ is $$\{1,\sqrt{5}\}$$, we know a basis for
$$E$$ over $$\mathbb Q$$ is given by the products

$$\{1\cdot 1, \sqrt{3}\cdot 1, 1\cdot \sqrt{5}, \sqrt{3}\cdot\sqrt{5}.$$

i.e. a basis is

$$\{1,\sqrt{3},\sqrt{5},\sqrt{15}\}.$$

