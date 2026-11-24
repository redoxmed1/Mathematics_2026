# Exercise 1. Recognizing Curves from Canonical Form

## Problem

Recognize the curves:

1. \ (x^2+y^2=9\)
3. \(\frac{x^2}{16}+\frac{y^2}{9}=1\)
4. \(y^2=8x\)
5. \(\frac{x^2}{9}-\frac{y^2}{4}=1\)

For each one, identify the most important features and make a sketch. Explain which parts of the equation let you recognize the type of curve.

## Solution

### 1. Circle: \(x^2+y^2=9\)

The standard circle equation is \(x^2+y^2=r^2\). Thus the center is \((0,0)\) and the radius is \(r=3\). Its intercepts are \((3,0),(-3,0),(0,3),(0,-3)\).

**Sketch (schematic):**
```text
             y
             ^
          .--|--.
        .'   |   '.
       /     |     \
------|------O------|----> x
       \     |     /
        '.   |   .'
          '--|--'
       -3    0    3
```

### 2. Ellipse: \(\frac{x^2}{16}+\frac{y^2}{9}=1\)

This is an ellipse centered at the origin. The semiaxis along the x-axis is \(a=4\), and the semiaxis along the y-axis is \(b=3\). The vertices are \((\pm4,0)\) and \((0,\pm3)\).

**Sketch (schematic):**
```text
             y
             ^
           .-|-.
        .-'  |  '-.
      .'     |     '.
-----+-------O-------+----> x
      '.     |     .'
        '-.  |  .-'
           '-|-'
       -4    0    4
```

### 3. Parabola: \(y^2=8x\)

Compare with \(y^2=4px\). Here \(4p=8\), so \(p=2\). The vertex is \((0,0)\), the axis is the x-axis, and the parabola opens to the right. Its focus is \((2,0)\) and directrix is \(x=-2\).

**Sketch (schematic):**
```text
             y
             ^
          \  |  /
           \ | /
            \|/
-------------O-----> x
            /|\
           / | \
          /  |  \
       opens right
```

### 4. Hyperbola: \(\frac{x^2}{9}-\frac{y^2}{4}=1\)

This is a horizontal hyperbola centered at \((0,0)\). Here \(a=3\), \(b=2\). Its vertices are \((\pm3,0)\), and its asymptotes are \(y=\pm\frac{2}{3}x\).

**Sketch (schematic):**
```text
             y
             ^
       \     |     /
        \   )| (  /
---------\--O--/----------> x
          \   /
          /   \
---------/-----\-----------
       two branches opening left and right
```

## Conclusion

The squared terms and their signs identify the curve: equal positive coefficients give a circle; unequal positive terms give an ellipse; one squared variable gives a parabola; and opposite signs give a hyperbola.
