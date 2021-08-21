# marginal likelihood

The marginal likelihood is obtained to [[marginalize]] a product of a [[prior]] distribution and a [[likelihood]] function for parameters, $\theta$.

## Definition

$$
p(\mathbf{X}) = \int_\theta p(\mathbf{X}|\theta) p(\theta) d\theta
$$

- $\mathbf{X} = \{ \mathbf{x}_1, \mathbf{x}_2, \cdots, \mathbf{x}_N \}, \mathbf{x}_i \in \mathbb{R}^M$: $\mathbf{X}$ is data of $N$ instances as $M$ dimensional vectors, $\mathbf{x}_i$ where $N, M \in \mathbb{N}$ 
- $\theta$: Parameters for a prior. 