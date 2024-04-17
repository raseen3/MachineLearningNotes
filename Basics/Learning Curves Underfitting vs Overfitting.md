# Learning Curves
plots that show changes in learning performance over time in terms of experience. They are typically used to visualize the performance of a machine learning model on the training and validation datasets over time or experience.

- **Training Curve**: Shows the performance of the model on the training dataset over time.
- **Validation Curve**: Shows the performance of the model on a validation dataset over time.

A model that is underfit will have high training and high testing error while an overfit model will have extremely low training error but a high testing error.

## Underfitting #underfitting
**Underfitting** occurs when a model is too simple to capture the underlying structure of the data.
### Symptoms
- Both training and validation errors are high.
- The model performs poorly on the training data.
### Causes
- Too simple model architecture.
- Not enough features.
- Too much regularization.
### Solutions
- Make the model more complex (use a more sophisticated model).
- Introduce more features or engineer existing ones.
- Reduce regularization.

## Overfitting #overfitting
**Overfitting** occurs when a model is too complex and starts to capture the noise in the data rather than the underlying structure.
### Symptoms
- Low training error but high validation error.
- The model performs very well on the training data but poorly on new, unseen data.
### Causes
- Too complex model architecture.
- Not enough training data.
- Little to no regularization.
### Solutions
- Simplify the model (use a less complex model).
- Get more training data.
- Increase regularization.
- Reduce the number of features.

## How to Calculate and Plot
1. **Split your data** into training and validation sets.
2. **For a range of training set sizes**:
    - Train your model on the current training set size.
    - Evaluate the model on the training data and record the error or accuracy.
    - Evaluate the model on the validation data and record the error or accuracy.
3. **Plot**:
    - Training set size (or iteration number) on the X-axis.
    - Performance metric (error or accuracy) on the Y-axis.
    - You'll have two lines: one for training performance and one for validation performance.
## How to Interpret
- **High Training and High Validation Error**:
    - The model is **underfitting**. It's too simple to represent the data well.
- **Low Training Error but High Validation Error**:
    - The model is **overfitting**. It's memorizing the training data rather than generalizing from it.
- **Converging Learning Curves**:
    - As more data is added, if the training and validation curves are converging, it indicates that adding more data might help improve the performance.
- **Diverging Learning Curves**:
    - If the validation error starts increasing while the training error is still decreasing, it's a clear sign of overfitting.