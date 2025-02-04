---
layout: page
title: Homework 2
permalink: /homework/hw2
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* written on ancient parchement with a quill and then flown to the instructor via owl post like in Harry Potter

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:**

Prove that if $$G$$ is a finite group and $$H\subseteq G$$ is a subset which is non-empty and closed under multiplication, then $$H$$ is a subgroup of $$G$$.

**Problem 2:**

Prove that the group $$\mathbb{Q}$$ with additive operation $$+$$ is not cyclic.

**Problem 3:**

* (a) Find all the subgroups of $$\mathbb{Z}_{10}$$
* (b) Find all values of $$n$$ for which there is a non-trivial group homomorphisms $$\mathbb{Z}_{10}\rightarrow Z_n$$
* (c) Find all values of $$n$$ for which there is a non-trivial group homomorphisms $$\mathbb{Z}_n\rightarrow Z_{10}$$

**Problem 4:**

For any $$a\in \mathbb{Z}_n$$, consider the function

$$f_a:\mathbb{Z}_n\rightarrow\mathbb{Z}_n,\quad f(x) = ax\mod n.$$

* (a) Prove that $$f_a$$ is a group homomorphism
* (b) Prove that if $$f: \mathbb{Z}_n\rightarrow\mathbb{Z}_n$$ is a group homomorphism, then $$f=f_a$$ for some $$a$$
* (c) Prove that $$f_a$$ is an automorphism if and only if $$\gcd(a,n) = 1$$
* (d) Prove that $$f_a\circ f_b = f_c$$ for $$c=ab\mod n$$

**Problem 5: **

The **cycle type** of a permutation $$\sigma\in S_n$$ is the size of the cycles
that make up the permutation when expressed as a product of disjoint cycles.  So for example, $$(543)$$ is a $$3$$-cycle, $$(12)(34)(567)$$ is a $$2,2,3$$-cycle, and so on.

* (a) Let $$\sigma\in S_n$$ and let $$(a_1a_2\dots a_r)$$ be an $$r$$-cycle.  Show that

$$\sigma(a_1a_2\dots a_r)\sigma^{-1}  = (\sigma(a_1)\sigma(a_2)\dots\sigma(a_r)).$$

* (b) Show that if $$f: S_n\rightarrow S_n$$ is an inner automorphism, then it preserves cycle types, ie. sends $$2$$-cycles to $$2$$-cycles, $$3,5$$-cycles to $$3,5$$-cycles, and so on.

**Problem 6:** Exotic embedding of $$S_5$$ into $$S_6$$.

Most monomorphism of $$S_5$$ into $$S_6$$ behave predictably in the sense that they send elements to other elements with the same cycle structure, so that for example, transpositions are sent to other transpositions.  However, by a freak algebraic coincidence there are others.
In this problem, we define a very unusual embedding of the group $$S_5$$ into the group $$S_6$$, called the **exotic embedding**.
It's construction touches on a number of important properties of groups we have discussed in class.

Consider all subgroups of $$S_5$$ of order $$5$$, ie.

$$
\begin{align*}
H_1 = \langle(12345)\rangle = \{e,(12345),(13524),(14253),(15432)\},\\
H_2 = \langle(12354)\rangle = \{e,(12354),(13425),(15243),(14532)\},\\
H_3 = \langle(12435)\rangle = \{e,(12435),(14523),(13254),(15342)\},\\
H_4 = \langle(12453)\rangle = \{e,(12453),(14325),(15234),(13542)\},\\
H_5 = \langle(12534)\rangle = \{e,(12534),(15423),(13245),(14352)\},\\
H_6 = \langle(12543)\rangle = \{e,(12543),(15324),(14235),(13452)\}.
\end{align*}
$$

* (a) Show that for any permutation $$\sigma\in S_5$$, there is a unique permutation $$\overline{\sigma}\in S_6$$ with

$$\sigma^{-1}H_k\sigma = H_{\overline\sigma(k)},\quad\text{for all}\ \ 1\leq k\leq 6.$$

* (b) Show that the function $$\psi: S_5\rightarrow S_6$$ defined by $$\psi(\sigma) = \overline{\sigma}$$ is a group monomorphism.

* (c) Show that $$\psi((45)) = (12)(35)(46)$$.  This shows that $$\psi$$ doesn't preserve cycle structure, demonstrating its exotic nature.

**Bonus Problem:** Exterior automorphism of $$S_6$$.

Using the exotic embedding from the previous problem, we can show that $$S_6$$ has an outer automorphism.
This is interesting, since it is the ONLY symmetric group which has an outer automorphism!

Let $$\overline H = \{\psi(\sigma): \sigma\in S_5\}$$.

* (a) Prove that $$\overline H$$ is a subgroup of $$S_6$$.
* (b) Show that the set $$S_6/\overline H$$ of left cosets of $$\overline H$$ in $$S_6$$ is

$$S_6/\overline H = \{C_1,C_2,C_3,C_4,C_5,C_6\}$$

where

$$C_1 = (16)\overline H,\ C_2 = (26)\overline H,\ \dots, C_6 = \overline H.$$

* (c) Prove that for every $$\sigma\in S_6$$, there exists a unique $$\widetilde\sigma\in S_6$$ with

$$\sigma C_j := \{\sigma x: x\in C_j\} = C_{\widetilde\sigma(j)}$$

* (d) Prove that the function $$\varphi: S_6\rightarrow S_6$$ defined by $$\varphi(\sigma) = \widetilde\sigma$$ is an automorphism
* (e) Show that $$\varphi((12)(35)(46))$$ has a different cycle type than $$(12)(35)(46)$$.  This shows that $$\varphi$$ is not an inner automorphism.




