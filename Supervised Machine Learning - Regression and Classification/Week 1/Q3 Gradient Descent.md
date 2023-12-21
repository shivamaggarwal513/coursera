# Gradient Descent

## Practice Quiz

### Question 1

Gradient descent is an algorithm for finding values of parameters w and b that minimize the cost function J.

$$
\text{repeat until convergence: }
\begin{cases}
    w = w - \alpha \frac{\partial J(w, b)}{\partial w} \\
    b = b - \alpha \frac{\partial J(w, b)}{\partial b}
\end{cases}
$$

When $\frac{\partial J(w, b)}{\partial w}$ is a negative number (less than zero), what happens to $w$ after one update step?

- $w$ decreases
- $w$ stays the same
- $w$ increases.
- It is not possible to tell if $w$ will increase or decrease.

Answer: C

Explanation: The learning rate is always a positive number, so if you take $w$ minus a negative number, you end up with a new value for $w$ that is larger (more positive).

### Question 2

For linear regression, what is the update step for parameter $b$?

- $b = b - \alpha \displaystyle\frac{1}{m}\displaystyle\sum_{i=1}^m \left(f_{w,b}(x^{(i)}) - y^{(i)}\right)$
- $b = b - \alpha \displaystyle\frac{1}{m}\displaystyle\sum_{i=1}^m \left(f_{w,b}(x^{(i)}) - y^{(i)}\right)x^{(i)}$

Answer: A

Explanation: The update step is $b = b - \alpha\frac{\partial J(w, b)}{\partial b}$ where $\frac{\partial J(w, b)}{\partial b}$ can be computed with this expression: $\displaystyle\frac{1}{m}\displaystyle\sum_{i=1}^m \left(f_{w,b}(x^{(i)}) - y^{(i)}\right)$
