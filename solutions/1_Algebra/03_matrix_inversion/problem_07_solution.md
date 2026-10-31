
### Exercise 7. Inverse of a Product

**Problem**

Given the matrices A and B:

Matrix A:

    | 1  1 |
    | 0  1 |

Matrix B:

    | 2  0 |
    | 0  3 |

Calculate the inverse of AB and calculate B inverse multiplied by A inverse. Check that both results are equal and explain why the inverse of a product reverses the order of the factors.

**Solution**

**1. Calculate AB**

Multiply the rows of A by the columns of B.

    AB =

    | 1(2) + 1(0)    1(0) + 1(3) |
    | 0(2) + 1(0)    0(0) + 1(3) |

Simplifying:

    AB =

    | 2  3 |
    | 0  3 |

**2. Calculate the inverse of AB**

First calculate the determinant:

    det AB = 2 × 3 - 3 × 0
           = 6

Since the determinant is nonzero, the inverse exists.

For a 2 × 2 matrix, the inverse formula is:

    | a  b | inverse = 1/(ad - bc) × |  d  -b |
    | c  d |                         | -c   a |

Applying the formula:

    AB inverse = 1/6 ×

    | 3  -3 |
    | 0   2 |

Therefore:

    AB inverse =

    |  1/2  -1/2 |
    |   0    1/3 |

**3. Calculate A inverse and B inverse separately**

For matrix A:

    det A = 1 × 1 - 1 × 0
          = 1

Therefore:

    A inverse =

    | 1  -1 |
    | 0   1 |

For matrix B:

    det B = 2 × 3 - 0 × 0
          = 6

Therefore:

    B inverse =

    | 1/2   0   |
    |  0   1/3  |

**4. Calculate B inverse multiplied by A inverse**

The inverse of a product requires reversing the order.

    B inverse × A inverse =

    | 1/2   0   |   | 1  -1 |
    |  0   1/3  | × | 0   1 |

Multiply rows by columns:

    | (1/2 × 1) + (0 × 0)     (1/2 × -1) + (0 × 1) |
    | (0 × 1) + (1/3 × 0)     (0 × -1) + (1/3 × 1) |

Simplifying:

    B inverse × A inverse =

    |  1/2  -1/2 |
    |   0    1/3 |

Both methods give exactly the same result.

    Inverse of AB =

    |  1/2  -1/2 |
    |   0    1/3 |

**5. Explain why the order is reversed**

When calculating ABx, matrix B acts on vector x first, and then matrix A acts on the result.

To undo these operations, we must reverse their order.

First, we undo A using A inverse.

Then, we undo B using B inverse.

The calculation is:

    A inverse × ABx = Bx

    B inverse × A inverse × ABx = x

Therefore:

    Inverse of AB = B inverse × A inverse

**Conclusion**

The inverse of a product reverses the order of the original matrices because the last transformation applied must be the first one undone.

The calculations confirm that both methods produce the same inverse matrix.


