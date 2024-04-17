As seen in [[Bayesian Learning]] we are given a Dataset or #evidence $D = \{x_1, x_2, \dots, x_n\}$
The Likelihood of the dataset is $P(D | w)$

## Maximum Likelihood Principle
the most likely explanation of $D$ is given by $\textbf{w}_{ML}$ which maximizes the likelihood function
$$
\textbf{w}_{ML} = arg max_{w}P(D | w)
$$
Assume Identically and Independently Distributed each $x_i \in D$ conditioned on $\textbf{w}$
$$
P(D | \textbf{w}) = P(D | \textbf{w}) = P(x_{1}, x_{2}, \dots , x_{n} | \textbf{w}) = \prod^{n}_{i = 1}{P(x_{i} | \textbf{w})}
$$
Maximize the log-likelihood then take the derivative and set it equal to 0.
$$
\textbf{w}_{ML} = arg max_{w} \prod^{n}_{i = 1} P(x_{i} | \textbf{w}) = arg max_{w} \sum^{n}_{i = 1} \log{P(x_{i} | \textbf{w})}
$$
$$
\frac{d}{dw} arg max_{w} \sum^{n}_{i = 1} \log{P(x_{i} | \textbf{w})} = 0
$$
