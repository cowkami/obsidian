# Bayes theorem

Let $x$ and $y$ be random variables, then they satisfy

$$
p(x|y) = \frac{p(y|x)p(x)}{p(y)}.
$$

This theorem can be easily obtained by a transformation of a joint probability equation as the following.

$$
\begin{split} \\
p(x, y) &= p(y, x) \\
\iff p(x|y)p(y) &= p(y|x)p(x)  \\
\iff p(x|y) &= \frac{p(y|x)p(x)}{p(y)}.
\end{split}
$$