## Poor Polynomials

We want to represent polynomials using lists, such that the coefficients are stored from the most significant to the least significant. That is, the polynomial

```haskell
  2x^3 - 3x^2 + 7
```

would be represented as

```haskell
  [2,-3,0,7]
```

Propose a data type, `Poly`, such that it exhibits the following behavior:

* (1 points) The toPoly function allows you to receive an arbitrary list of numbers and "convert" it into a Poly.
* (1 points) The Show instance shows the polynomials in algebraic notation instead of a simple list.
* (1 point) The `addPoly p0 p1` function allows adding two polynomials.
* (2 points) The `evalPoly p x` function allows to evaluate the value of the polynomial `p` at point `x`.

You cannot use `length` or `reverse` in its implementation. To obtain all the points, the implementation of each function has to make a single pass through the list that internally represents the polynomial.
