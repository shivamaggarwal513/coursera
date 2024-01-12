# Recommender Systems Implementation

## Graded Quiz

### Question 1

Lecture described using 'mean normalization' to do feature scaling of the ratings. What equation below best describes this algorithm?

-

$$
\begin{aligned}
y_{\text{norm}}(i, j) &= \frac{y(i,j)-\mu_i}{\sigma_i} \text{, where} \\
\mu_i &= \frac{1}{\sum_j r(i,j)} \sum_{j:r(i,j)=1} y(i,j) \\
\sigma_i^2 &= \frac{1}{\sum_j r(i,j)} \sum_{j:r(i,j)=1} (y(i,j)-\mu_j)^2 \\
\end{aligned}
$$

-

$$
\begin{aligned}
y_{\text{norm}}(i, j) &= y(i,j)-\mu_i \text{, where} \\
\mu_i &= \frac{1}{\sum_j r(i,j)} \sum_{j:r(i,j)=1} y(i,j) \\
\end{aligned}
$$

-

$$
\begin{aligned}
y_{\text{norm}}(i, j) &= \frac{y(i,j)-\mu_i}{\max_i-\min_i} \text{, where} \\
\mu_i &= \frac{1}{\sum_j r(i,j)} \sum_{j:r(i,j)=1} y(i,j) \\
\end{aligned}
$$

Answer: B

Explanation: This is the mean normalization algorithm described in lecture. This will result in a zero average value on a per-row basis.

### Question 2

The implementation of collaborative filtering utilized a custom training loop in TensorFlow. Is it true that TensorFlow always requires a custom training loop?

- No. TensorFlow provides simplified training operations for some applications.
- Yes. TensorFlow gains flexibility by providing the user primitive operations they can combine in many ways.

Answer: A

Explanation: Recall in Course 2, you were able to build a neural network using a `model`, `compile`, `fit` sequence which managed the training for you. A custom training loop was utilized in this situation because training $w$, $b$, and $x$ does not fit the standard layer paradigm of TensorFlow's neural network flow. There are alternate solutions such as custom layers, however, it is useful in this course to introduce you to this powerful feature of TensorFlow.

### Question 3

Once a model is trained, the 'distance' between features vectors gives an indication of how similar items are.

The squared distance between the two vectors $\mathbf{x}^{(k)}$ and $\mathbf{x}^{(i)}$ is:

$\text{distance} = \left\Vert \mathbf{x}^{(k)} - \mathbf{x}^{(i)} \right\Vert^2 = \displaystyle\sum_{l=1}^{n} \left(x_l^{(k)} - x_l^{(i)}\right)^2$

Using the table below, find the closest item to the movie "Pies, Pies, Pies".

| Movie               | User 1 | ... | User n | $x_0$ | $x_1$ | $x_2$ |
| :------------------ | :----- | :-- | :----- | :---: | :---: | :---: |
| Pastries for Supper |        |     |        | 2.0   | 2.0   | 1.0   |
| Pies, Pies, Pies    |        |     |        | 2.0   | 3.0   | 4.0   |
| Pies and You        |        |     |        | 5.0   | 3.0   | 4.0   |

- Pastries for Supper
- Pies and You

Answer: B

Explanation: The distance from 'Pies, Pies, Pies' is $9 + 0 + 0 = 9$.

### Question 4

Which of these is an example of the cold start problem? (Check all that apply.)

- A recommendation system is unable to give accurate rating predictions for a new product that no users have rated.
- A recommendation system is unable to give accurate rating predictions for a new user that has rated few products.
- A recommendation system takes so long to train that users get bored and leave.
- A recommendation system is so computationally expensive that it causes your computer CPU to heat up, causing your computer to need to be cooled down and restarted.

Answer: AB

Explanation: A recommendation system uses product feedback to fit the prediction model. A recommendation system uses user feedback to fit the prediction model.
