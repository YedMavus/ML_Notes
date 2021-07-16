# Week 1 Lecture 4: Evaluation and Cross Validation

Given a hypothesis space H and training data S, the learning algo comes up with a function h. To understand how good the h is, we need to evaluate it using experimental evaluation, ie having a metric using which we evaluate, eg 
- error metric
- accuracy
- precision and recall

These evaluations are done on the training set or even better a seperate test set.

Given y' = h(x) is a prediction on x and y is the actual value. If y' differs from y, we have an error.

Types of errors:
- Absoloute error: 
  - 1/n &sum;{|h(x) - y|}
- Sum of Square Method: 1/n &sum;(h(x) - y)<sup>2</sup>
- Classification error: 1/n &sum; &delta; (h(x),y)

In classification, we define a confusion matrix
|Hyp Class\True Class | Positive | Negative |
|.|.|.|
|Positive|True Positive[TP]|False Positive[FP]|
|Negative| False Negative[FN]| True Negative[TN] |
| | P | N |

Obviously the diagonal elements are either all true or all false

Accuracy = TP + TN/ P + N
\\How many are correctly predicted
Precision = TP/ TP + FP
\\Answers how many are correctly positive
Recall = TP / P
How many of the positive examples are retrieved as positive, also called true positive rate. False positive rate also exists.
