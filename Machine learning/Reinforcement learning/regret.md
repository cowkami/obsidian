# Regret

In [[Multi-armed bandit]] problem, we can use [[regret]] as a criterion to maximize reward.

## Cumulative regret

Suppose there is a bandit machine that has $K$ arms. An agent has $K$ actions and repeats $n \in \{1, 2, \cdots, T\}$ trials for $T$ times.
Each arm has a mean reward $\mu_i$, $i \in \{ 1, 2, \cdots, K \}$, and some of them have a maximum mean reward, $\mu^*$.
 
### Definition

$$
R_n = \sum_{t=1}^{n} \mu^* - \mu_{I(t)}
$$

- $\mu_i$: mean reward
- $\mu^*$: maximum mean reward
- $I(n)$: a selection policy that outputs some at time n


## References

[1] Tom Pepels et al., "Minimizing Simple and Cumulative Regret in Monte-Carlo Tree Search" (2014)