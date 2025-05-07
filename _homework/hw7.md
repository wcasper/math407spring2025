---
layout: page
title: Homework 7
permalink: /homework/hw7
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* written on ancient parchement with a quill and then flown to the instructor via owl post like in Harry Potter

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:**

Suppose that $$K$$ is a splitting field of $$f(x)\in F[x]$$ and that $$\sigma: K\rightarrow K$$ is a field automorphism.
Prove that if $$\sigma(a) = a$$ for all $$a\in F$$ and $$\sigma(r) = r$$ for all $$r\in K$$ with $$f(r) = 0$$, then $$\sigma$$ is the identity function.


**Problem 2:**

Suppose that $$K$$ is the splitting field of $$f(x)\in F[x]$$, and that $$f(x)$$ is a degree $$n$$ polynomial with $$n$$ distinct roots $$r_1, r_2,\dots, r_n$$.
* (a) Prove that if $$\sigma\in\text{Gal}_F(K)$$, then $$\sigma$$ restricts to a permutation of the set $$\{r_1,\dots, r_n\}$$.
* (b) Prove that $$\text{Gal}_{\mathbb Q}(F)$$ is isomorphic to a subgroup of $$S_n$$.
* (c) Prove that $$r_1 + r_2 + \dots + r_n$$ must be an element of $$F$$.

**Problem 3:**

Let $$K$$ be the splitting field of $$x^3-5$$ and let $$\omega =e^{2\pi i/3}$$.
* (a) Prove that the set

$$\{1, \sqrt[3]{5}, \sqrt[3]{5^2},\omega, \sqrt[3]{5}\omega, \sqrt[3]{5^2}\omega\}$$

is a basis for $$K$$ as a $$\mathbb Q$$-vector space. [Hint: first show that $$K = \mathbb Q(\sqrt[3]{5},\omega)$$]

* (b)  Prove that the $$\mathbb Q$$-linear transformation defined on the basis above by

$$\begin{align*}
\sigma:  & a_0 + b_0\sqrt[3]{5} + c_0\sqrt[3]{5^2} + a_1\omega + b_1\sqrt[3]{5}\omega + c_1\sqrt[3]{5^2}\omega\\
         &\mapsto a_0 - b_1\sqrt[3]{5} - c_1\sqrt[3]{5^2} + a_1\omega + (b_0-b_1)\sqrt[3]{5}\omega + (c_0-c_1)\sqrt[3]{5^2}\omega
\end{align*}$$

is a field automorphism of $$K$$.

* (c) Show that complex conjugation $$\delta(z) = \overline{z}$$ restricts to a field automorphism of $$K$$

* (d) Determine the Galois group $$\text{Gal}_{\mathbb Q}(K)$$.  What "standard" group is it isomorphic to?

**Problem 4:**

Let $$n>1$$ be an integer, $$\omega_n = e^{2\pi i/n}\in\mathbb{C}$$ and consider the field $$K = \mathbb Q(\omega_n)$$.
* (a) Prove that $$K$$ is a splitting field.
* (b) If $$\sigma\in \text{Gal}_{\mathbb Q}(\mathbb C)$$, prove that  $$\sigma(\omega_n) = \omega_n^a$$ for some integer $$1\leq a < n$$ relatively prime to $$n$$.
* (c) Prove that 

$$1 + e^{2\pi i/n} + e^{4\pi i/n} + e^{6\pi i/n} + \dots + e^{2(n-1)\pi i/n}$$

is a rational number.  What number is it?

**Problem 5:**

Suppose that $$K$$ is a splitting field over a field $$F$$ and that $$u\in K$$, and let

$$\text{Gal}_F(K) = \{\sigma_1,\sigma_2,\dots,\sigma_n\}.$$

* (a) Prove that the polynomial

$$f(x) = (x-\sigma_1(u))(x-\sigma_2(u))\dots (x-\sigma_n(u))$$

is a polynomial in $$F[x]$$ which has $$u$$ as a root.

* (b) Find a polynomial with $$\sqrt{2} + \sqrt{3} + \sqrt{5}$$ as a root.








