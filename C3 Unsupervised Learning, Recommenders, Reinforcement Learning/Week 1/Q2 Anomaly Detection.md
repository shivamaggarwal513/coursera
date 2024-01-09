# Anomaly Detection

## Graded Quiz

### Question 1

You are building a system to detect if computers in a data center are malfunctioning. You have 10,000 data points of computers functioning well, and no data from computers malfunctioning. What type of algorithm should you use?

- Anomaly detection
- Supervised learning

Answer: A

Explanation: Creating an anomaly detection model does not require labeled data.

### Question 2

You are building a system to detect if computers in a data center are malfunctioning. You have 10,000 data points of computers functioning well, and 10,000 data points of computers malfunctioning. What type of algorithm should you use?

- Anomaly detection
- Supervised learning

Answer: B

Explanation: You have a sufficient number of anomalous examples to build a supervised learning model.

### Question 3

Say you have 5,000 examples of normal airplane engines, and 15 examples of anomalous engines. How would you use the 15 examples of anomalous engines to evaluate your anomaly detection algorithm?

- You cannot evaluate an anomaly detection algorithm because it is an unsupervised learning algorithm.
- Use it during training by fitting one Gaussian model to the normal engines, and a different Gaussian model to the anomalous engines.
- Because you have data of both normal and anomalous engines, don't use anomaly detection. Use supervised learning instead.
- Put the data of anomalous engines (together with some normal engines) in the cross-validation and/or test sets to measure if the learned model can correctly detect anomalous engines.

Answer: D

Explanation: Anomalous examples are used to evaluate rather than train the model.

### Question 4

Anomaly detection flags a new input $x$ as an anomaly if $p(x) < \epsilon$. If we reduce the value of $\epsilon$, what happens?

- The algorithm is more likely to classify new examples as an anomaly.
- The algorithm is less likely to classify new examples as an anomaly.
- The algorithm is more likely to classify some examples as an anomaly, and less likely to classify some examples as an anomaly. It depends on the example $x$.
- The algorithm will automatically choose parameters $\mu$ and $\sigma$ to decrease $p(x)$ and compensate.

Answer: B

Explanation: When $\epsilon$ is reduced, the probability of an event being classified as an anomaly is reduced.

### Question 5

You are monitoring the temperature and vibration intensity on newly manufactured aircraft engines. You have measured 100 engines and fit the Gaussian model described in the video lectures to the data. The 100 examples and the resulting distributions are shown in the figure below.

![Probability](./images/C3_W1_Q1_Probability.png)

The measurements on the latest engine you are testing have a temperature of 17.5 and a vibration intensity of 48. These are shown in magenta on the figure below. What is the probability of an engine having these two measurements?

- $17.5 \times 48 = 840$
- $0.0738 \times 0.02288 = 0.00169$
- $0.0738 + 0.02288 = 0.0966$
- $17.5 + 48 = 65.5$

Answer: B

Explanation: According to the model described in lecture, $p(A, B) = p(A) . p(B)$.
