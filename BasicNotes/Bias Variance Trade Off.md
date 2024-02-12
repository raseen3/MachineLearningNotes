# Bias Variance

## Bias #bias 
**Definition**: The inability for a machine learning method to capture the true relationship
Bias measure how far off in general a model's prediction is from the correct value.
### High Bias 
- is when the model oversimplifies (pays little attention to training data) which lead to high error. This is known as underfitting #underfitting 
### Low Bias 
- focuses a lot of attention to the training data and is useless for anything other than the training data

## Variance #variance 
**Definition**: the difference/variability in fits between datasets and the model
### High Variance 
- is when the model fits closely to the training data and can't not be generalized to any other dataset resulting in high errors or overfitting #overfitting 
### Low Variance 
- model will produce similar predictions consistently across different training sets.

## Trade-off #trade-off
There's a trade-off between bias and variance. Improving bias (making the model more flexible) tends to increase variance and vice versa. This is visually represented by the "Bias-Variance Tradeoff" graph, which shows that the total error of a model (usually measured as Mean Squared Error) is minimized when we find the right balance of bias and variance. Too much flexibility leads to overfitting (high variance), while too little flexibility leads to underfitting (high bias).

### Goal
In machine learning, the ultimate aim is to choose a model with both low bias and low variance. However, in practice, decreasing bias increases variance and vice versa. This trade-off leads to the dilemma of selecting the right level of model complexity. The optimal balance typically results in the best model performance on unseen data.