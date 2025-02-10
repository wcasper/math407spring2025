---
layout: page
title: Practice Exam 1 Solutions
permalink: /exams/practice-exam1-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.

a) if $$G$$ is not Abelian and $$H\leq G$$, then $$H$$ is not Abelian

b) If $$H$$ and $$K$$ are subgroups of a group $$G$$, then the intersection $$H\cap K$$ is also a subgroup of $$G$$

c) If $$G$$ is a group of order $$4$$, then $$G$$ must be a cyclic group

d) If $$H$$ is a subgroup of a finite group $$G$$, then the number of left cosets of $$H$$ in $$G$$ must divide the order of $$G$$

e) If $$G$$ is a group and $$a\in G$$, then $$a^2 = a$$ if and only if $$a=e$$

**Solution:**

F,T,F,T,T

## Problem 2

Let $$G$$ and $$H$$ be groups with identities $$e_G$$ and $$e_H$$, respectively, and suppose that $$f: G\rightarrow H$$ is a group homomorphism.

a) Prove that $$f(e_G) = e_H$$.
b) Prove that $$f(a^{-1}) = f(a)^{-1}$$.
c) Prove that the image of $$\varphi$$

$$\text{img}(f) = \{f(a): a\in G\}$$

is a subgroup of $$H$$

**Solution:**

a) $$f(e_G) = f(e_G*e_G) = f(e_G)*f(e_G)$$, so that $$f(e_G) = f(e_G)^2$$.  This means

$$e_H = f(e_G)^{-1}f(e_G) = f(e_G)^{-1}f(e_G)^2 = f(e_G).$$

b) From part (a)

$$e_H = f(e_G) = f(aa^{-1}) = f(a)f(a^{-1}).$$

Therefore $$e_H  = f(a)f(a^{-1})$$ and it follows

$$f(a)^{-1} = f(a)^{-1}e_H = f(a)^{-1}(f(a)f(a^{-1})) = (f(a)^{-1}f(a))f(a^{-1}) = e_Hf(a^{-1}) = f(a^{-1}).$$

c) From part (a), $$\text{img}(f)$$ is non-empty since it contains $$e_H$$.

Suppose $$b,d\in \text{img}(f)$$.  Then there exists $$a,c\in G$$ with $$b=f(a)$$ and $$d=f(c)$$.  Therefore

$$bd = f(a)f(c) = f(ac)\in\text{img}(f).$$

This proves that $$\text{img}(f)$$ is closed under multiplication.

Lastly, since $$G$$ is a group $$a^{-1}\in G$$ and by part (b)

$$b^{-1} = f(a)^{-1} = f(a^{-1}) \in\text{img}(f).$$

Thus $$\text{img}(f)$$ is closed under inversion, showing that it is a subgroup.


## Problem 3

Let $$G$$ be a cyclic group.
Show that every subgroup of $$G$$ is also cyclic.

**Solution:**

Since $$G$$ is cyclic, there exists $$a\in G$$ with

$$G = \{a^k: k\in\mathbb{Z}\}.$$

Suppose that $$H\leq G$$.  If $$H = \{e\}$$, then $$H$$ is cyclic, so without loss of generality, we may assume $$H$$ contains a non-identity element.
Consider the set

$$K = \{k\in\mathbb{Z}: k \geq 1,\ \ a^k\in H\}.$$

Since $$G$$ contains more than the identity, $$K$$ is non-empty.
By the Well Ordering Principle, it therefore has a minimal element $$d$$.
In particular $$a^d\in H$$, and therefore $$\langle a^d\rangle \subseteq H$$.

We claim that this inclusion is actually an equality!
To see this, suppose $$h\in H$$.
Then $$h\in G$$ so $$h = a^k$$ for some $$k\in \mathbb{Z}$$.
We consider three cases:
* Case 1: $$k > 0$$.  Then $$k \geq d$$ by the definition of $$d$$.
Therefore by the division algorithm, we can write $$k = pd + q$$ for some integers $$p$$ and $$q$$ with $$0\leq q < d$$.
Consequently $$a^q = h(a^{d})^{-p}\in H$$, and from the definition of $$d$$ we must have that $$q=0$$.
Therefore $$k = pd$$ and $$h = (a^d)^p\in \langle a^d\rangle$$.
* Case 2: $$k < 0$$.  Then since $$H$$ is a subgroup $$h^{-1} = a^{-k}\in H$$ also.  By the previous argument $$h^{-1}\in \langle a^d\rangle$$, and consequently $$h\in \langle a^d\rangle$$ since $$\langle a^d\rangle$$ is a group
* Case 3: $$k=0$$.  Then $$h = e\in \langle a^d\rangle$$.

Thus in any case, we have $$h\in \langle a^d\rangle$$, and this proves $$H = \langle a^d\rangle$$.

## Problem 4

Let $$G = \mathbb Z_8$$.

a) Determine explicitly the elements of $$\text{Aut}(G)$$.

b) Prove that $$\text{Aut}(G)$$ is isomorphic to the Klein four group $$\mathbb{Z}_2\times\mathbb{Z}_2$$.

**Solution:**

a) As we saw in class and in the homework,

$$\text{Aut}(G) = \{f_a: a\in\mathbb{Z}_8,\ \gcd(a,8) = 1\},$$

where here $$f_a: \mathbb{Z}_8\rightarrow\mathbb{Z}_8$$ is the function $$f_a(x) = ax\mod 8$$.
Therefore

$$\text{Aut}(G) = \{f_1,f_3,f_5,f_7\}.$$

b) Recall $$f_a\circ f_b = f_{ab}$$.  Therefore $$f_1\circ f_1 = f_1$$, $$f_3\circ f_3 = f_1$$, $$f_5\circ f_5 = f_1$$, and $$f_7\circ f_7= f_1$$.
In particular $$\text{Aut}(G)$$ has no elements of order $$4$$, and therefore cannot be isomorphic to $$\mathbb{Z}_4$$.
We showed in class that up to isomorphism the only other group of order $$4$$ is the Klein $$4$$-group, so $$G$$ must be isomorphic to that group.

## Problem 5

Prove that if $$G$$ is a group and $$\lvert G\rvert$$ is a prime number, then $$G$$ is a cyclic group.

**Solution:**

Suppose that $$\lvert G\rvert = p$$ for some prime number $$p$$, and let $$a\in G$$ with $$a\neq e$$.
Then the cyclic subgroup $$\langle a\rangle$$ of $$G$$ has more than one element.
By Lagrange's Theorem, the order of $$\langle a\rangle$$ must divide $$p$$, so we conclude that $$\langle a\rangle$$ has $$p$$ elements.
Hence $$G = \langle a\rangle$$.

## Problem 6

Consider the set

$$G=\{(a,b): \text{$a,b$ integers},\ 0\leq a < 7,\ 0\leq b < 3\}$$

with the associative binary operation

$$(a,b)\ast (c,d)  = (a +_7 (2^bc), b +_3 d).$$

For example
$$(3,2)*(5,1) = (3 +_7 (2^25),2+_31) = (3 +_7 20, 0) = (2,0).$$

a) Show that $$G$$ has an identity element

b) Show each element of $$G$$ has an inverse

c) Show that $$G$$ is not Abelian

d) Find the order of the element $$(1,1)$$ in $$G$$.  Show your work.

**Solution:**

a) $$(a,b)\ast (0,0) = (a,b)$$ and $$(0,0)\ast (a,b) = (a,b)$$ so $$(0,0)$$ is an identity for $$G$$

b) 

$$(a,b)\ast (4^b6a,2b) = (a +_7 (2^b4^b6a), b+_32b) = (a +_7 (8^b6a),3b) = (a +_7(6a),0) = (7a,0) = (0,0).$$

Likewise 

$$(4^b6a,2b)\ast (a,b) = (4^b6a +_7 2^{2b}a, 2b+_3b) = (2^{2b}6a +_7 2^{2b}a, 3b) = (2^{2b}7a,0) = (0,0).$$

Therefore the inverse of $$(a,b)$$ is $$(4^b6a,2b)$$.

c) $$(1,0)\ast (1,1) = (1+_72^01,0+_31) = (2,1)$$ and $$(1,1)\ast(1,0) = (1+_72^11,1+_30) = (3,1)$$.  Therefore the group is non-Abelian

d) 

$$(1,1)\ast (a,b) = (1+_72^1a,1+_3a) = (2a+_71,a+_31)$$

Therefore

$$\begin{align*}
(1,1)^2 = (1,1)\ast (1,1) &= (3,2)\\
(1,1)^3 = (1,1)\ast (3,2) &= (0,0).
\end{align*}$$


Thus $$(1,1)$$ has order $$3$$.

## Problem 7

A group $$G$$ is called **divisible** if given any $$x\in G$$ andy any integer $$n>0$$ there exists a $$y\in G$$ so that $$y^n=x$$.

[Remember: $$y^n$$ means $$y*y*y*\dots*y$$ $$n$$ times, where $$*$$ is the binary operation of the group $$G$$.]

a) Show that the group $$\mathbb Q$$ (with binary operation addition) is divisible.

b) Show that if $$G$$ is a nontrivial cyclic group, then $$G$$ cannot be divisible.


**Solution:**

a) Careful!  Since the binary operation is addition $$y^n = y*y*\dots *y$$ really means $$y+y+\dots+y=ny$$.
Therefore what we are trying to show is that given any $$x,\in \mathbb{Q}$$ and integer $$n>0$$ there exists a $$y\in\mathbb{Q}$$ with $$ny = x$$.

Let $$x\in\mathbb{Q}$$ and let $$n>1$$ be an integer.
Then $$x$$ is rational, so $$y=x/n$$ is also rational, meaning $$y\in\mathbb{Q}$$.
Moreover $$ny = n(x/n) = x$$, so we are done.

b) Let $$G$$ be a nontrivial cyclic group and assume that $$G$$ is divisible.  Then $$G = \langle a\rangle$$ for some $$a\in G$$ with $$a\neq e$$.
If $$G$$ is divisible, then there must exist $$y\in G$$ with $$y^2=a$$.
Moreover since $$a$$ generates $$G$$, we know $$y =a^k$$ for some integer $$k$$.
Therefore $$a^{2k} = a$$, which implies $$G$$ is a finite group.

Let $$d=\lvert G\rvert$$.  Then as a consequence of Lagrange's Theorem $$x^d=e$$ for all $$x\in G$$.  However since $$G$$ is a divisible group, there must also be a $$z\in G$$ with $$z^d = a$$.  This implies $$a=e$$, which is a contradiction.


