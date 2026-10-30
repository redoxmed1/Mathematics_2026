### Exercise 13. A Recurrence Written in Matrix Form

**Problem**

Let

$$
F=\begin{pmatrix}1&1\\1&0\end{pmatrix}.
$$

Compute F², F³, F⁴, and F⁵. Compare the entries with the Fibonacci sequence 0, 1, 1, 2, 3, 5, 8, … . Then compute F(a, b)ᵀ and explain one recurrence step.

**Solution**

**Calculate F² row by column.**

$$
F^2=\begin{pmatrix}
1(1)+1(1) & 1(1)+1(0) \\
1(1)+0(1) & 1(1)+0(0)
\end{pmatrix}=\begin{pmatrix}2&1\\1&1\end{pmatrix}.
$$

**Calculate F³ row by column.**

$$
F^3=F^2F=\begin{pmatrix}
2(1)+1(1) & 2(1)+1(0) \\
1(1)+1(1) & 1(1)+1(0)
\end{pmatrix}=\begin{pmatrix}3&2\\2&1\end{pmatrix}.
$$

**Calculate F⁴ row by column.**

$$
F^4=F^3F=\begin{pmatrix}
3(1)+2(1) & 3(1)+2(0) \\
2(1)+1(1) & 2(1)+1(0)
\end{pmatrix}=\begin{pmatrix}5&3\\3&2\end{pmatrix}.
$$

**Calculate F⁵ row by column.**

$$
F^5=F^4F=\begin{pmatrix}
5(1)+3(1) & 5(1)+3(0) \\
3(1)+2(1) & 3(1)+2(0)
\end{pmatrix}=\begin{pmatrix}8&5\\5&3\end{pmatrix}.
$$

The entries are consecutive Fibonacci numbers. With F₀ = 0 and F₁ = 1, the pattern is

$$
F^n=\begin{pmatrix}F_{n+1}&F_n\\F_n&F_{n-1}\end{pmatrix},\qquad n\geq1.
$$

For example, F⁵ contains F₆ = 8, F₅ = 5, and F₄ = 3. The row-by-column calculations show that each new entry is the sum of two appropriate neighboring Fibonacci numbers.

**One recurrence step.**

$$
F\begin{pmatrix}a\\b\end{pmatrix}=\begin{pmatrix}1(a)+1(b)\\1(a)+0(b)\end{pmatrix}=\begin{pmatrix}a+b\\a\end{pmatrix}.
$$

The new first entry is the sum of the previous two values, and the second entry retains a. This makes the vector ready for the next recurrence step.
