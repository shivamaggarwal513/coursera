# Continuous State Spaces

## Graded Quiz

### Question 1

The Lunar Lander is a continuous state Markov Decision Process (MDP) because:

- The state contains numbers such as position and velocity that are continuous valued.
- The reward contains numbers that are continuous valued.
- The state has multiple numbers rather than only a single number (such as position in the $x$-direction).
- The state-action value $Q(s,a)$ function outputs continuous valued numbers.

Answer: A

### Question 2

In the learning algorithm described in the videos, we repeatedly create an artificial training set to which we apply supervised learning where the input $x=(s,a)$ and the target, constructed using Bellman’s equations, is $y=\underline{\qquad}$?

- $y=\displaystyle\max_{a'} Q(s',a')$ where $s'$ is the state you get to after taking action $a$ in state $s$.
- $y=R(s) + \gamma \displaystyle\max_{a'} Q(s',a')$ where $s'$ is the state you get to after taking action $a$ in state $s$.
- $y=R(s)$
- $y=R(s')$ where $s'$ is the state you get to after taking action $a$ in state $s$.

Answer: B

### Question 3

You have reached the final practice quiz of this class! What does that mean? (Please check all the answers, because all of them are correct!)

- What an accomplishment -- you made it!
- The DeepLearning.AI and Stanford Online teams would like to give you a round of applause!
- Andrew sends his heartfelt congratulations to you!
- You deserve to celebrate!

Answer: ABCD
