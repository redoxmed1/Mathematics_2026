# Ćwiczenie 1 – Rozmiar i elementy macierzy

## Problem

Dane są następujące macierze:

$$
A = \begin{pmatrix} 
2 & -1 & 3 \\\\ 
0 & 4 & 5 
\end{pmatrix}
$$

$$
B = \begin{pmatrix} 
1 & 0 \\\\ 
-2 & 3 \\\\ 
4 & 1 
\end{pmatrix}
$$

1. Podaj rozmiary macierzy $A$ i $B$.
2. Odczytaj elementy $a_{12}$, $a_{23}$, $b_{21}$ oraz $b_{32}$.
3. Zapisz drugi wiersz macierzy $A$ oraz pierwszą kolumnę macierzy $B$ jako wektory.

---

## Rozwiązanie

### Krok 1: Określenie rozmiarów macierzy

Rozmiar macierzy określa liczba wierszy pomnożona przez liczbę kolumn ($m \times n$).
- Macierz $A$ ma 2 wiersze i 3 kolumny.
- Macierz $B$ ma 3 wiersze i 2 kolumny.

Dlatego:

$$
\text{Rozmiar } A = 2 \times 3, \qquad \text{Rozmiar } B = 3 \times 2
$$

---

### Krok 2: Odczytanie wskazanych elementów

W zapisie $a_{ij}$ lub $b_{ij}$ pierwszy indeks $i$ oznacza wiersz, a drugi indeks $j$ oznacza kolumnę:

- $a_{12}$ znajduje się w 1. wierszu i 2. kolumnie macierzy $A$:

$$
a_{12} = -1
$$

- $a_{23}$ znajduje się w 2. wierszu i 3. kolumnie macierzy $A$:

$$
a_{23} = 5
$$

- $b_{21}$ znajduje się w 2. wierszu i 1. kolumnie macierzy $B$:

$$
b_{21} = -2
$$

- $b_{32}$ znajduje się w 3. wierszu i 2. kolumnie macierzy $B$:

$$
b_{32} = 1
$$

---

### Krok 3: Zapisanie wskazanych wektorów wierszowych i kolumnowych

- Drugi wiersz macierzy $A$ zapisany jako wektor wierszowy:

$$
\text{Drugi wiersz } A = \begin{pmatrix} 0 & 4 & 5 \end{pmatrix}
$$

- Pierwsza kolumna macierzy $B$ zapisana jako pionowy wektor kolumnowy:

$$
\text{Pierwsza kolumna } B = \begin{pmatrix} 1 \\\\ -2 \\\\ 4 \end{pmatrix}
$$

---

## Wnioski

- Macierz $A$ ma rozmiar $2 \times 3$, a macierz $B$ ma rozmiar $3 \times 2$.
- Szukane elementy to $a_{12} = -1$, $a_{23} = 5$, $b_{21} = -2$ oraz $b_{32} = 1$.
- Drugi wiersz $A$ to $\begin{pmatrix} 0 & 4 & 5 \end{pmatrix}$, a pierwsza kolumna $B$ to pionowy wektor $\begin{pmatrix} 1 \\\\ -2 \\\\ 4 \end{pmatrix}$.
