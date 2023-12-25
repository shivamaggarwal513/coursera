# Cost Function for Logistic Regression

## Graded Quiz

### Question 1

In this lecture series, "cost" and "loss" have distinct meanings. Which one applies to a single training example?

$$
J(\mathbf{w}, b) = \frac{1}{m} \sum_{i=1}^{m} L\left(f_{\mathbf{w}, b}\left(\mathbf{x}^{(i)}\right), y^{(i)}\right)
$$

- Loss
- Cost
- Both Loss and Cost
- Neither Loss nor Cost

Answer: A

Explanation: In these lectures, loss is calculated on a single training example. It is worth noting that this definition is not universal. Other lecture series may have a different definition.

### Question 2

For the simplified loss function, if the label $y^{(i)} = 0$, then what does this expression simplify to?

$$
L\left(f_{\mathbf{w}, b}(\mathbf{x}^{(i)}), y^{(i)}\right) =
\begin{cases}
    - \log \left(f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right) & \text{if } y^{(i)} = 1 \\
    - \log \left(1 - f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right) & \text{if } y^{(i)} = 0
\end{cases}
$$

$$
L\left(f_{\mathbf{w}, b}(\mathbf{x}^{(i)}), y^{(i)}\right) = -y^{(i)} \log \left(f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right) - \left(1 - y^{(i)}\right) \log \left(1 - f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right)
$$

- $- \log \left(1 - f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right) - \log \left(1 - f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right)$
- $\log \left(1 - f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right) + \log \left(1 - f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right)$
- $\log \left(f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right)$
- $- \log \left(1 - f_{\mathbf{w}, b}(\mathbf{x}^{(i)})\right)$

Answer: D

Explanation: When $y^{(i)} = 0$, the first term reduces to zero.
