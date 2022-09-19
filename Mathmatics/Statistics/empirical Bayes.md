# Empirical Bayes

Empirical Bayes is a method to determine hyperparameters of priors from data.
By maximizing the [[marginal likelihood]] for hyperparameters, then we can obtain hyperparameters given data.

Let $\eta$ be hyperparameters of prior, $p(\theta|\eta)$ then it can be obtained empirical hyperparameters, $\hat{\eta}$ as

$$
\hat{\eta} = \arg\max\limits_{\eta} \,p(X|\eta) = \int_\theta p(X|\theta) p(\theta|\eta) \,d\theta.
$$

If we execute full Bayes inference, it is required to calculate [[marginal likelihood]] over both $\theta$ and $\eta$ as

$$
p(X) = \int_{\theta, \eta} p(X|\theta) p(\theta|\eta) p(\eta) \,d\theta \,d\eta ,
$$

but it is analytically intractable.

[[evidence approximation]]
[[type 2 maximum likelihood]]
