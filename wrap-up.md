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

## 2. Curve fitting

(Lecture05)


### 2.1 Interpolation

### 2.2 Regression
