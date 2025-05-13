---
layout: page
title: Practice Final Solutions
permalink: /exams/practice-final-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)

Let $$F$$ be a field, $$E$$ an extension field of $$F$$ and $$G = \text{Gal}_F(E)$$

* (a) $$F$$ is the fixed subfield of $$G$$, ie. $$F = \{a\in E: \sigma(a) = a\ \forall a\in G\}$$

FALSE!  For this to be true, we need to assume that $$E$$ is nice enough, ie. the splitting field of a separable polynomial.

* (b) If $$f(x)\in F[x]$$ and $$a\in E$$ is a root of $$f(x)$$, then $$\sigma(a)$$ is also a root of $$f(x)$$

TRUE!  In fact $$0 = \sigma(0) = \sigma(f(a)) = f(\sigma(a))$$.

* (c) If $$F\subseteq E$$ is a Galois extension, then $$\lvert G\rvert = [E:F]$$

TRUE!  This was a Theorem from class.  Remember, think of Galois extensions as more or less splitting fields of separable polynomials.

* (d) If $$f(x)\in F(x)$$ is irreducible, then all of the roots of $$f(x)$$ must be different

FALSE!  The example from class was where $$F = \mathbb Z_p(t)$$ is the field of rational functions with coefficients in $$\mathbb Z_p$$ for some prime $$p$$.  Then the polynomial $$f(x) = x^p-t\in F[x]$$ is irreducible by Eisenstein's criterion but **all** of the roots are the same and equal to $$\sqrt[p]{t}$$.  This is the most basic example of this kind of behavior, but is an important example to remember!

* (e) If $$F\subseteq E$$ is a Galois extension, then the number of subgroups of $$G$$ is equal to the number of field extensions of $$F$$ contained in $$E$$

True!  This follows from Galois Corresponence.

## Problem 2

* (a) State what it means for a field extension to be normal.  Give an explicit example of a field extension which is normal, and one which is not normal.

A field extension $$F\subseteq E$$ is called normal if every polynomial $$f(x)\in F[x]$$ which has a root in $$E$$ actually splits over $$E$$.
Any splitting field is normal, so for example $$\mathbb Q(\sqrt{2})$$ is normal.
The field $$E = \mathbb Q(\sqrt[3]{2})$$ is NOT normal, since the polynomial $$x^3-2$$ has a root in $$E$$ but does not split over $$E$$.

* (b) State the First Isomorphism Theorem for rings.

Let $$\varphi: R\rightarrow S$$ be a morphism of rings and let $$I=\ker(\varphi)$$.  Then the map

$$\overline\varphi: R/I\rightarrow \text{img}(\varphi),\quad r + I\mapsto \varphi(r)$$

is an isomorphism of rings.

* (c) Write down the definition of an ideal $$I$$ of a commutative ring $$R$$.

An ideal $$I\subseteq R$$ is a subset of $$R$$ which is
* non-empty
* closed under addition
* has the property that if $$a\in I$$ and $$r\in R$$ then $$ra\in I$$

* (d) Give an example of a field extension $$E$$ of a field $$F$$ whose Galois group is $$\mathbb Z_2\times\mathbb Z_2$$.

Let $$E$$ be the splitting field of $$f(x) = (x^2-2)(x^2-3)$$ over $$F = \mathbb Q$$.
Then since $$E = \mathbb Q(\sqrt{2},\sqrt{3}) = \mathbb Q(\sqrt{2})(\sqrt{3})$$, we know that $$[E:F] = 4$$ so the Galois group has order $$4$$.
If $$\sigma\in\text{Gal}_F(E)$$, then
$$\sigma(\sqrt{2}) = \pm\sqrt{2}$$ and $$\sigma(\sqrt{3}) = \pm\sqrt{3}$$.
Therefore $$\sigma^2(\sqrt{2}) = \sqrt{2}$$ and $$\sigma^2(\sqrt{3}) = \sqrt{3}$$, and consequently $$\sigma^2 = \text{id}$$.
Thus every element of the Galois group has order $$2$$ and we conclude $$\mathbb Z_2\times\mathbb Z_2$$.

## Problem 3

Consider the field extension $$K = \mathbb Q(\sqrt[4]{2},i)$$ of $$F=\mathbb Q$$.

* (a) Prove that $$K$$ is the splitting field of a polynomial.

The splitting field of the polynomial $$x^4-2$$ is $$E = \mathbb Q(\sqrt[4]{2},-\sqrt[4]{2}, \sqrt[4]{2}i,-\sqrt[4]{2}i)$$.
Since $$\sqrt[4]{2}\in E$$ and $$i = (\sqrt[4]{2}i)/(\sqrt[4]{2})\in E$$, we have $$K\subseteq E$$.
Conversely, $$\sqrt[4]{2},-\sqrt[4]{2}, \sqrt[4]{2}i,-\sqrt[4]{2}i\in K$$, so $$E\subseteq K$$.
Thus $$E=K$$, which shows that $$K$$ is a splitting field.

* (b) Prove that $$[K:F] = 8$$ and therefore $$\text{Gal}_F(K)$$ has order $$8$$

First, the minimal polynomial of $$\sqrt[4]{2}$$ over $$\mathbb Q$$ is $$x^4-2$$, so $$[\mathbb Q(\sqrt[4]{2}):\mathbb Q] = 4$$.
In fact a basis for $$\mathbb Q(\sqrt[4]{2})$$ as a vector space over $$\mathbb Q$$ is

$$\{1,\sqrt[4]{2},\sqrt[4]{4},\sqrt[4]{8}\}.$$

Next, the minimal polynomial of $$i$$ over $$\mathbb Q(\sqrt[4]{2})$$ is $$x^4-2$$, so $$K=\mathbb Q(\sqrt[4]{2})(i)$$ satisfies $$[K:\mathbb Q(\sqrt[4]{2})] = 2$$.
In fact a basis for $$K$$ over $$\mathbb Q(\sqrt[4]{2})$$ is $$\{1,i\}$$.

Thus

$$[K: Q] = [K:\mathbb Q(\sqrt[4]{2})][\mathbb Q(\sqrt[4]{2}):\mathbb Q] = 2\cdot 4 = 8$$

and in fact a basis for $$K$$ over $$\mathbb Q$$ is given by

$$\{1,\sqrt[4]{2},\sqrt[4]{4},\sqrt[4]{8},i,i\sqrt[4]{2},i\sqrt[4]{4},i\sqrt[4]{8}\}$$

* (c) Prove that there exists $$\sigma\in \text{Gal}_F(K)$$ satisfying $$\sigma(\sqrt[4]{2}) = i\sqrt[4]{2}$$.  Explain why $$\sigma$$ has order $$4$$

Since $$K$$ is the splitting field of a separable polynomial, and both $$\sqrt[4]{2}$$ and $$\sqrt[4]{2}i$$ are roots of the same minimal polynomial $$x^4-2$$, a theorem from class tells us there is an element $$\sigma\in\text{Gal}_{\mathbb Q}(K)$$ satisfying $$\sigma(\sqrt[4]{2}) = i\sqrt[4]{2}$$.

* (d) Prove that complex conjugation $$\tau: K\rightarrow K$$, $$\tau(z) = \overline{z}$$ is also an element of $$\text{Gal}_F(K)$$

A basis for $$K$$ over $$\mathbb Q$$ is

$$\{1,\sqrt[4]{2},\sqrt[4]{4},\sqrt[4]{8},i,i\sqrt[4]{2},i\sqrt[4]{4},i\sqrt[4]{8}\}$$

Therefore if $$z\in K$$, we have

$$z = a_1 + b_1\sqrt[4]{2} + c_1\sqrt[4]{4} + d_1\sqrt[4]{8} + ia_2 + i\sqrt[4]{2}b_2 +i\sqrt[4]{4}c_2 + i\sqrt[4]{8}d_2$$

for some rational numbers $$a_j,b_j,c_j,d_j$$.
This means that the complex conjugate

$$\overline z = a_1 + b_1\sqrt[4]{2} + c_1\sqrt[4]{4} + d_1\sqrt[4]{8} - ia_2 - i\sqrt[4]{2}b_2 - i\sqrt[4]{4}c_2 - i\sqrt[4]{8}d_2$$

also belongs to $$K$$.  Consequently complex conjugation $$\tau: \mathbb C\rightarrow\mathbb C$$,  $$\tau(z) = \overline{z}$$ restricts to a function $$\tau: K\rightarrow K$$.

Since $$\tau(zw) = \overline{zw} = \overline z\overline w = \tau(z)\tau(w)$$ and $$\tau(z+w) = \overline{z+w} = \overline z + \overline w = \tau(z) + \tau(w)$$, we also know that $$\tau$$ is a field homomorphism.
Finally, since $$\tau^2=\text{id}$$, $$\tau$$ is its own inverse function and is therefore bijective.  Hence $$\tau\in\text{Gal}_F(K)$$

* (e) Show that $$\text{Gal}_F(K) = \langle \sigma,\tau\rangle$$ and $$\text{Gal}_F(K)\cong D_4$$

We calculate

$$\sigma(\tau(\sqrt[4]{2})) = \sigma(\sqrt[4]{2}) = i\sqrt{4}{2}$$

and also

$$\tau(\sigma(\sqrt[4]{2})) = \tau(i\sqrt{4}{2}) = -i\sqrt{4}{2}$$

which shows that $$\sigma\tau\neq \tau\sigma$$.  Therefore $$\text{Gal}_{\mathbb Q}(K)$$ is a non-Abelian group of order $$8$$.
This means that it is either $$D_4$$ or the quaternions.
We can tell the quaternions and $$D_4$$ apart in several ways, the simplest being the fact that the quaternions only have a single element of order $$2$$.
In contrast $$D_4$$ has four elements of order $$2$$.

The order of $$\sigma$$ cannot be $$1$$ (since it's not the identity) or $$8$$ (since the Galois group is non-Abelian and hence not cyclic).
Therefore it is either $$2$$ or $$4$$.
If the order of $$\sigma$$ is $$2$$, then $$\sigma$$ and $$\tau$$ are two different elements of order $$2$$.
If the order of $$\sigma$$ is $$4$$, then $$\sigma^2$$ and $$\tau$$ are two different elements of order $$2$$.
In either case, we have multiple elements of order $$2$$, so the Galois group is $$D_4$$.

## Problem 4

Let $$R = \mathbb{Z}[x]$$ be the ring of polynomials with integer coefficients and let $$I$$ be the ideal of $$R$$ generated by $$5$$ and $$x^2+2x+1$$.
Describe explicitly the cosets of $$R/I$$.  How many are there?

Let $$f(x)\in\mathbb{Z}[x]$$.
By the division algorithm, we can write

$$f(x) = (x^2+x+1)q(x) + r(x)$$

where here $$q(x),r(x)\in\mathbb Z[x]$$ with $$\deg(r(x)) < 2$$.
It follows that

$$f(x)\equiv r(x)\mod I.$$

Furthermore, since $$\deg r(x)\leq 1$$ we can write $$r(x) = ax + b$$ for some $$a,b\in \mathbb{Z}$$.
Again, by the division algorithm 

$$a = 5a_0 + a_1\quad\text{and}\quad b = 5b_0 + b_1$$

for some integers $$a_0,a_1,b_0,b_1$$ with $$0\leq a_1,b_1 < 5$$.
Therefore 

$$f(x) = 5(a_0x + b_0) + a_1x + b_1\equiv a_1x+b_1\mod I.$$

It follows that every polynomial in $$R/I$$ is equivalent to a polynomial of the form $$a_1x + b_1$$ where $$0\leq a_1,b_1 < 5$$.
The cosets of $$R/I$$ are thus

$$R/I = \{(a_1x+b_1) + I: 0\leq a_1,b_1 < 5\}$$

and there are $$25$$ such elements.


## Problem 5

* (a) State Lagrange's theorem

Let $$G$$ be a finite group and $$H$$ be a subgroup.  Then $$\lvert G\rvert = [G:H]\cdot\lvert H\rvert$$

* (b) Suppose that $$G$$ is a non-cyclic group of order $$27$$.  Prove that $$g^9=e$$ for all $$g\in G$$

Let $$g\in G$$ and let $$d$$ be the order of $$g$$.
Then by Lagrange's theorem the order of the subgroup $$\langle g\rangle$$ must divide the order of $$G$$.
Therefore $$d$$ must be $$1,3,9$$ or $$27$$.
Since $$G$$ is non-Abelian, it can't be cyclic so the order of $$g$$ cannot be $$27$$.
Hence the order $$d$$ of $$g$$ is $$1$$, $$3$$, or $$9$$.  In any case $$d$$ divides $$9$$ and so

$$g^9 = (g^d)^{9/d} = e^{9/d} = e.$$

* (c) Determine, up to isomorphism, all the finite Abelian groups of order $$72$$

Since $$72 = 2^3\cdot 3^2$$, the non-isomorphic Abelian groups are

$$\mathbb{Z}_2\times \mathbb{Z}_2\times \mathbb{Z}_2\times\mathbb Z_3\times\mathbb Z_3$$

$$\mathbb{Z}_4\times \times \mathbb{Z}_2\times\mathbb Z_3\times\mathbb Z_3$$

$$\mathbb{Z}_8\times\mathbb Z_3\times\mathbb Z_3$$

$$\mathbb{Z}_2\times \mathbb{Z}_2\times \mathbb{Z}_2\times\mathbb Z_6$$

$$\mathbb{Z}_4\times \times \mathbb{Z}_2\times\mathbb Z_6$$

$$\mathbb{Z}_8\times\mathbb Z_6$$

## Problem 6

Let

$$G = \{(a,b)\in \mathbb Q\times\mathbb Q: a\neq 0\}.$$

Show that the binary relation

$$(a,b)*(c,d) = (ac,ad + bc)$$

is well-defined and makes $$G$$ into a group.

We must show associativity.

$$((a,b)*(c,d))*(e,f) = (ac,ad + bc)(e,f) = (ace, acf + ade + bce)$$

$$(a,b)*((c,d)*(e,f)) = (a,b)(ce, cf + de) = (ace, acf + ade + bce)$$

Since these are the same, we have associativity.

Next, we need an identity element.  Since

$$(a,b)*(1,0) = (a,b),\quad\text{and}\quad (1,0)*(a,b) = (a,b)$$

the element $$(1,0)$$ is an identity element.

Lastly, we need to show that we have inverses.

Since

$$(a,b)*(1/a, -b/a^2) = (1,0),\quad\text{and}\quad (1/a, -b/a^2)*(a,b) = (1,0)$$

we see that $$(1/a, -b/a^2)$$ is an inverse of $$(a,b)$$.
Hence we have inverses, making $$G$$ a group.


## Problem 7

Consider the field extension $$K = \mathbb Q(\omega_{21})$$ of $$F=\mathbb Q$$, where $$\omega_{n} = \exp(2\pi i/n)$$.
Recall from class that 

$$\text{Gal}_F(K) = \{\sigma_m: 1\leq m < 21,\ \gcd(m,21) = 1\}$$

where here $$\sigma_m: K\rightarrow K$$ is a field automorphism satisfying $$\sigma_m(\omega_n) = \omega_n^m$$

* (a) Prove that $$K$$ is the splitting field of a polynomial.

Since the roots of $$x^{21}-1$$ are $$1,\omega_{21},\omega_{21}^2,\dots, \omega_{21}^{20}$$

$$K = \mathbb Q(\omega_{21}) = \mathbb Q(1,\omega_{21},\omega_{21}^2,\dots,\omega_{21}^{20})$$

we see that $$K$$ is a splitting field of $$x^{21}-1$$.

* (b) Consider the element

$$u = \omega_{21} + \omega_{21}^2 + \omega_{21}^4 + \omega_{21}^8 + \omega_{21}^{16} + \omega_{21}^{11}.$$

What subgroup of $$\text{Gal}_F(K)$$ does the intermediate field $$F(u)$$ correspond to?

We need to figure out which of the automorphisms fix the element $$u$$.
The Galois group is

$$\{\sigma_1,\sigma_2,\sigma_4,\sigma_5,\sigma_8,\sigma_{10},\sigma_{11},\sigma_{13},\sigma_{16},\sigma_{17},\sigma_{19},\sigma_{20}\}$$

and has $$12$$ elements.

Since $$\sigma_2(u) = u$$, we have that $$\sigma_{2}^k(u) = u$$ for all $$k$$.  Therefore $$u$$ is fixed by $$\sigma_2^k = \sigma_{2^k}$$ for all $$k$$, ie. all the elements in the subgroup.

$$H = \{\sigma_1,\sigma_2,\sigma_4,\sigma_8,\sigma_{16},\sigma_{11}\}.$$

By Lagrange's theorem any larger group would be the entire Galois group.  However $$u$$ isn't fixed by everything.  Thus the subgroup corresonding to the intermediate field is $$H$$.

* (c) Consider the subgroup $$H = \langle \sigma_4, \sigma_{20} \rangle$$ of $$\text{Gal}_F(K)$$.  What subfield of $$K$$ does $$H$$ correspond to?

Now we need to figure out the subfield $$E$$ of $$K$$ fixed by all the elements of $$H$$.
The group $$H$$ has $$6$$ elements, so we expect $$[E:F] = [\text{Gal}_F(K):H] = 2$$.

The element

$$v = \omega_{21} + \omega_{21}^4 + \omega_{21}^{16} + \omega_{21}^{-1} + \omega_{21}^{-4} + \omega_{21}^{-16}$$

is fixed by all the elements of $$H$$ but not by all of the elements of $$\text{Gal}_F(K)$$.
Therefore it is an element of $$E$$ not in $$F$$.  Since $$[E:F]=2$$, it follows that $$E = F(v)$$.

