VC Dimension, named after Vapnik and Chervonenkis, is a fundamental concept in the theory of statistical learning. It provides a measure of the capacity or complexity of a classification model, specifically the capacity of a hypothesis class to fit data. The VC Dimension helps in understanding overfitting, generalization, and the relation between bias and variance.

**Formal Definition**: The VC Dimension of a hypothesis class $\mathcal{H}$ is the largest size of a set that can be shattered by $\mathcal{H}$. If a hypothesis class can shatter sets of arbitrarily large size, then its VC Dimension is said to be infinite.

**Shattering**: A hypothesis class $\mathcal{H}$ is said to shatter a set of points if, for every possible labeling of those points into two classes (positive/negative or 0/1), there exists some hypothesis in $\mathcal{H}$ that separates the points according to that labeling. In other words, for every possible dichotomy of the set, there's a hypothesis in $\mathcal{H}$ that captures that dichotomy perfectly.

**Why is VC Dimension Important?**:

1. **Model Complexity**: VC Dimension gives a measure of the complexity of a model. A higher VC Dimension indicates a more complex model.
2. **Generalization**: It provides a bound on the generalization error of a classifier. A model with a high VC Dimension might have a low training error but might not generalize well to unseen data.
3. **Overfitting**: Models with high VC Dimensions are more prone to overfitting, especially when the number of training samples is small.
4. **Bias-Variance Tradeoff**: VC Dimension plays a role in understanding the tradeoff between bias and variance. A high VC Dimension might lead to low bias but high variance.

**Examples**:

1. For a linear classifier in a 2D plane (like the perceptron), the VC Dimension is 3. This means that any set of 3 points in the plane can be shattered by a linear classifier, but there exists a set of 4 points that cannot be shattered.
2. For a decision stump (a one-level decision tree), the VC Dimension is 2.
3. For more complex models, the VC Dimension can be much higher or even infinite.

In practice, while VC Dimension provides theoretical insights into the capacity of models, it's often challenging to compute for complex models. However, understanding the concept is crucial for grasping the fundamentals of statistical learning theory.