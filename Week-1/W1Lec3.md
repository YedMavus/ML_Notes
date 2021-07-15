# Hypothesis Space and Inductive Bias

## Inductive Learing or Prediction
- Given examples or data of form (x , y) / (x, f(x))
  - **Classification Problems:** f(x) is discrete
  - **Regression Problems**: f(x) is continuous
  - **Probability Estimation:** f(x) is the probability of x
**
Why inductive learning**: Given data, use induction, as opposed to deduction, to try and identify a function that predicts the data.

Features: Properties that describe each instance

If multiple features, use feature vector.

### Feature Space

Recall Vector Space

For n features, we define a n fimentional "feature" space, similar to vector spaces. Each instance becomes a point in the feature space.

Take a 2 class classification problem.
We have 2 types of instances.
Training set has subset of instances - some marked class 1{denoted by +1} , others 2{denoted by -1}.

We can map different points in the feature set. We want a function to predict, for a new instance, whether it is a + or - . 
It could be a curve or line that seperates an area in the feature space (2D, so area). This is what inductive learning is. Points to the left of this line is positive, to the right are negative, for example. The line is a hypothesis that we use to do the prediction. 
It needn't be a linear function. It could be a polynomial curve, or even a decision tree. These are just representations. Neural Networks are also another representation.


**Hypothesis space**: Class of functions that can in principle be output by the learning algorithm.
