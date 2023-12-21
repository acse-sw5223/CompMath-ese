# Wrap-up

## 1. Error

(Lecture04)

### 1.1 Norms

A norm on some space is a function which assigns to every entry in that space a size.

- $ \| v \|_2 = \sqrt{v_1^2 + v_2^2 + \ldots + v_n^2} = \left(\sum_{i=1}^n v_i^2 \right)^{1/2}$, two-norm, Euclidean norm

- $ \| v \|_1 = |v_1| + |v_2| + \ldots + |v_n| = \sum_{i=1}^n |v_i|$, one-norm, taxi-cab or Manhattan norm

- $ \| v \|_{\infty} = \max\{|v_1|,|v_2|, \ldots, |v_n| \} = \max_{i=1}^n |v_i|$, max-norm

### 1.2 Log-log error plot

**If** we plot data using log-log axes and **if** we get a straight line then we know the underlying function must be of the form $\, y = ax^k $, where we can estimate $k$ by finding the slope of the line.

Similarly, if we get *approximately* a straight line, of *approximate* slope $k$, then we know that $\, y \approx ax^k $.  

Or, if we approach a straight line of splope $p$ in some limit say, then we know that $\, y = \mathcal{O}(x^p) $ in that limit.  This is our case from above.

## 2. Curve Approximation

(Lecture05)

### 2.1 Interpolation

Interpolation generally assumes that these **data points are exact** (e.g. no measurement errors) and at distinct $x$ locations, i.e. there is no ambiguity in a mapping from $x$ to $y$.

The process of interpolation then seeks to fit a function (or curve),

$$ y = f(x), $$

to this data that exactly passes through the $N+1$ discrete points.

Given the data our job in interpolation is to find a suitable function $f$. We can then use this function to find (or estimate) $y$ values at $x$ locations other than those provided by the data.

Types:

- Polynomials (Lagrange polynomials, Chebyshev and Hermite polynomials, and splines)
- Piecewise polynomials
- Trigonometric series (Fourier series)

### 2.2 Regression (Curve fitting)

In this case we do not have an explicit group of points in order, and can consider the data simply as a *cloud of points*, not worrying what order they are in.

### 2.3 Quadrature

Numerical evaluation of a definite integral.

#### 2.3.1 Midpoint Rule

Also called the rectangle method.

$$I_M := \sum_{i=0}^{n-1} \, f \left ( \frac {x_{i+1}+x_i} {2} \right )\, (x_{i+1}-x_i).$$

#### 2.3.2 Trapezodial Rule

Change the shape of the rectangle to a trapezoid (i.e. the top of the shape now being a linear line fit defined by the values of the function at the two end points of the subinterval, rather than the constant value used in the midpoint rule), we arrive at the trapezoid, or trapezoidal, rule.

$$I_T := \sum_{i=0}^{n-1}\, \left(\frac{f(x_{i+1}) + f(x_{i})}{2}\right )\, (x_{i+1}-x_i). $$

#### 2.3.3 Simpson's Rule

## 3. ODE

(Lecture07)

## 4. PDE

(Lecture08)
