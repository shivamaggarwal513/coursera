# Regression

## Practice Quiz

### Question 1

For linear regression, the model is $f_{w,b}(x) = wx + b$. Which of the following are the inputs, or features, that are fed into the model and with which the model is expected to make a prediction?

- $x$
- $m$
- $(x, y)$
- $(w, b)$

Answer: A

Explanation: The $x$, the input features, are fed into the model to generate a prediction $f_{w, b}(x)$.

### Question 2

For linear regression, if you find parameters $(w, b)$ so that $J(w, b)$ is very close to zero, what can you conclude?

- The selected values of the parameters $(w, b)$ cause the algorithm to fit the training set really poorly.
- This is never possible -- there must be a bug in the code.
- The selected values of the parameters $(w, b)$ cause the algorithm to fit the training set really well.

Answer: C

Explanation: When the cost is small, this means that the model fits the training set well.
