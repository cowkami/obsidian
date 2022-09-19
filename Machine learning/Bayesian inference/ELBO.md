# ELBO(Evidence Lower BOund)

In Bayesian inference, we often want to maximize log [[evidence]]

## Definition

$$
\mathbf{ELBO} \equiv \mathbb{E}_{q_\phi(\mathbf{z})} \left[ \log{p_\theta(\mathbf{x}, \mathbf{z})} - \log{q_\phi(\mathbf{z})} \right]
$$

- $\mathbf{x}$: random variable
- $\mathbf{z}$: [[latent variable]]
- $q_\phi(\mathbf{z})$: a distribution parameterized by $\phi$