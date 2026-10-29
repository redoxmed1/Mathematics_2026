### Exercise 13. A Recurrence Written in Matrix Form

**Problem**

Let

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}.
$$

Compute F², F³, F⁴, and F^5. Compare the numbers obtained with the sequence 0,1,1,2,3,5,8,… and describe the relationship. Then compute F\beginpmatrixa; b\endpmatrix and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

**Solution**

**1. Calculate the powers**

$$
F^2=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}.
$$

$$
F^3=F^2F=
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}.
$$

$$
F^4=F^3F=
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}.
$$

$$
F^5=F^4F=
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}.
$$

The entries follow consecutive Fibonacci numbers. With F_0=0 and F_1=1, the powers have the pattern

$$
F^n=
\begin{pmatrix}
F_{n+1} & F_n \\
F_n & F_{n-1}
\end{pmatrix}
$$

for n≥ 1. For example, F^5 contains 8, 5, 5, and 3, which are consecutive Fibonacci numbers.

**2. One recurrence step**

Multiply F by a vector:

$$
F
\begin{pmatrix}
a \\
b
\end{pmatrix}
=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
a \\
b
\end{pmatrix}
=
\begin{pmatrix}
a+b \\
a
\end{pmatrix}.
$$

The new vector contains the sum a+b and the previous first value a. If a and b are consecutive terms, this produces the next term and retains the preceding one, so the recurrence can continue.

---
