### Exercise 3. When is a matrix product defined?

## Question

The matrices have dimensions

$$
A:2\times3,\qquad B:3\times4,\qquad
C:4\times2,\qquad D:2\times2.
$$

Determine whether each product \(AB\), \(BA\), \(BC\), \(CB\), \(AC\), \(CA\), \(AD\), and \(DA\) is defined. For every defined product, give its dimensions.

## Solution

For a product \(XY\), the number of columns of \(X\) must equal the number of rows of \(Y\). If \(X\) is \(m\times n\) and \(Y\) is \(n\times p\), then \(XY\) is defined and has size \(m\times p\): the matching inner dimensions \(n\) are checked, while the outer dimensions give the result.

1. **\(AB\):** \(A\) is \(2\times3\) and \(B\) is \(3\times4\). The inner dimensions match, \(3=3\), so \(AB\) is defined and has size \(2\times4\).

2. **\(BA\):** \(B\) is \(3\times4\) and \(A\) is \(2\times3\). The inner dimensions are \(4\) and \(2\), which do not match. Thus \(BA\) is not defined.

3. **\(BC\):** \(B\) is \(3\times4\) and \(C\) is \(4\times2\). The inner dimensions match, \(4=4\), so \(BC\) is defined and has size \(3\times2\).

4. **\(CB\):** \(C\) is \(4\times2\) and \(B\) is \(3\times4\). The inner dimensions are \(2\) and \(3\), which do not match. Thus \(CB\) is not defined.

5. **\(AC\):** \(A\) is \(2\times3\) and \(C\) is \(4\times2\). The inner dimensions are \(3\) and \(4\), which do not match. Thus \(AC\) is not defined.

6. **\(CA\):** \(C\) is \(4\times2\) and \(A\) is \(2\times3\). The inner dimensions match, \(2=2\), so \(CA\) is defined and has size \(4\times3\).

7. **\(AD\):** \(A\) is \(2\times3\) and \(D\) is \(2\times2\). The inner dimensions are \(3\) and \(2\), which do not match. Thus \(AD\) is not defined.

8. **\(DA\):** \(D\) is \(2\times2\) and \(A\) is \(2\times3\). The inner dimensions match, \(2=2\), so \(DA\) is defined and has size \(2\times3\).
