# Bayesian Learning

## Probability
$P(A = a)$ is the probability that hypothesis $A = a$ is true.
You can chain conditions together to get a **Joint Distribution** 
$$
P(A = a \land B = b)
$$
Conditional Probability is getting the probability of a condition being true given that a different condition is true
$$
P(A | B) = \frac{P(A \land B)}{P(B)}
$$
### Bayes Rule #bayes-rule
$$
P(B | A) = \frac{P(A | B) P(B)}{P(A)}
$$
- Form a **[[Hypothesis]]** $H$ about the world based on what we **observe** using **[[Evidence]]** $e$
$$
P(H | e) = \frac{P(e | H) P(H)}{P(e)}
$$
#### Prior Probability
- $P(H)$ is the **Prior Probability** of $H$ #prior-probability
#### Likelihood
- $P(e | H)$ is the **Likelihood** of $e$ given $H$ #likelihood
#### Evidence
- $P(e)$ is the **Normalizing Constant** or **Evidence** for $e$ #evidence
#### Posterior Probability
- $P(H | e)$ is the **Posterior Probability** of $H$ #posterior-probability
