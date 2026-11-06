# Ćwiczenie 5 – Iloczyn macierzy przez wektor

## Problem

Niech

$$
A =
\begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix}
$$

$$
x =
\begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

Oblicz $Ax$. Następnie wyraź $Ax$ jako kombinację liniową kolumn macierzy $A$, gdzie współczynnikami są składowe wektora $x$.

---

## Rozwiązanie

### Krok 1: Mnożenie macierzy przez wektor

Pomnóż każdy wiersz macierzy $A$ przez wektor kolumnowy $x$:

$$
Ax =
\begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

Oblicz poszczególne elementy:

$$
Ax =
\begin{pmatrix}
(2)(4) + (-1)(2) \\
(1)(4) + (3)(2)
\end{pmatrix}
$$

Uprość arytmetykę:

$$
Ax =
\begin{pmatrix}
6 \\
10
\end{pmatrix}
$$

---

### Krok 2: Wyrażenie wyniku za pomocą kolumn

Niech pierwsza i druga kolumna macierzy $A$ będą oznaczone jako $a_1$ i $a_2$:

$$
a_1 =
\begin{pmatrix}
2 \\
1
\end{pmatrix}
$$

$$
a_2 =
\begin{pmatrix}
-1 \\
3
\end{pmatrix}
$$

Współrzędne wektora $x$ to $4$ i $2$, więc iloczyn macierzy i wektora można zapisać jako kombinację liniową $4a_1 + 2a_2$:

$$
Ax = 4
\begin{pmatrix}
2 \\
1
\end{pmatrix}
+ 2
\begin{pmatrix}
-1 \\
3
\end{pmatrix}
$$

Wykonaj mnożenie przez skalar:

$$
Ax =
\begin{pmatrix}
8 \\
4
\end{pmatrix}
+
\begin{pmatrix}
-2 \\
6
\end{pmatrix}
$$

Dodaj wektory współrzędna po współrzędnej:

$$
Ax =
\begin{pmatrix}
6 \\
10
\end{pmatrix}
$$

---

## Wnioski

- Bezpośredni iloczyn macierzy i wektora wynosi:

$$
Ax =
\begin{pmatrix}
6 \\
10
\end{pmatrix}
$$

- Przedstawiony jako kombinacja liniowa kolumn macierzy $A$ przy użyciu składowych wektora $x$:

$$
4
\begin{pmatrix}
2 \\
1
\end{pmatrix}
+ 2
\begin{pmatrix}
-1 \\
3
\end{pmatrix}
=
\begin{pmatrix}
6 \\
10
\end{pmatrix}
$$

Potwierdza to, że pomnożenie macierzy przez wektor daje kombinację liniową jej kolumn.
