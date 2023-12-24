# Gradient Descent for Logistic Regression

## Graded Quiz

### Question 1

$$\text{Gradient Descent for Logistic Regression}$$

$$
\text{repeat until convergence: }
\begin{cases}
    w_j = w_j - \alpha \left[\displaystyle\frac{1}{m} \displaystyle\sum_{i=1}^m \left(f_{\mathbf{w}, b}\left(\mathbf{x}^{(i)}\right) - y^{(i)}\right)x_j^{(i)}\right] \\
    b = b - \alpha \left[\displaystyle\frac{1}{m} \displaystyle\sum_{i=1}^m \left(f_{\mathbf{w}, b}\left(\mathbf{x}^{(i)}\right) - y^{(i)}\right)\right]
\end{cases}
$$

$$
f_{\mathbf{w}, b}\left(\mathbf{x}^{(i)}\right) = \frac{1}{1 + e^{-(\mathbf{w} \cdot \mathbf{x} + b)}}
$$

Which of the following two statements is a more accurate statement about gradient descent for logistic regression?

- The update steps are identical to the update steps for linear regression.
- The update steps look like the update steps for linear regression, but the definition of $f_{\mathbf{w}, b}\left(\mathbf{x}^{(i)}\right)$ is different.

Answer: B

Explanation: For logistic regression, $f_{\mathbf{w}, b}\left(\mathbf{x}^{(i)}\right)$ is the sigmoid function instead of a straight line.
