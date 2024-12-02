# Exam Review Exercises

1. Gini Impurity: Calculate the Gini impurity for a dataset $D$ with 40 instances of class A and 60 instances of class B.

   - $$Gini(D) = ... $$

2. Given the following dataset with two attributes (Feature1 and Feature2) and a class label, use the Naïve Bayes classifier to predict the class label of a new sample (Feature1 = 3, Feature2 = 7).

   | Feature1 | Feature2 | Class Label |
   | -------- | -------- | ----------- |
   | 1        | 5        | A           |
   | 2        | 6        | A           |
   | 3        | 8        | B           |
   | 4        | 7        | B           |
   | 2        | 5        | A           |

3. Given the following confusion matrix, calculate Precision, Recall, and F1 Score.

   |                 | Predicted Positive | Predicted Negative |
   | --------------- | ------------------ | ------------------ |
   | Actual Positive | 20                 | 5                  |
   | Actual Negative | 10                 | 30                 |

4. A probabilistic classifier has been applied to a test set of 10 tuples. Below are the probability values of these tuples belonging to the positive class, sorted in decreasing order. Based on these probabilities and the actual class labels, calculate the True Positive Rate (TPR) and False Positive Rate (FPR) at each threshold, and then sketch the ROC curve.

   | Probability | Actual Class |
   | ----------- | ------------ |
   | 0.90        | Positive     |
   | 0.85        | Positive     |
   | 0.80        | Negative     |
   | 0.75        | Positive     |
   | 0.70        | Negative     |
   | 0.65        | Negative     |
   | 0.60        | Positive     |
   | 0.55        | Negative     |
   | 0.50        | Positive     |
   | 0.45        | Negative     |

5. Given a dataset with 5 tuples {A, B, C, D, E} and their distance matrix as shown below, perform two rounds of Agglomerative Clustering.

   |       | **A** | **B** | **C** | **D** | **E** |
   | ----- | ----- | ----- | ----- | ----- | ----- |
   | **A** | 0.00  | 2.24  | 4.12  | 7.07  | 7.00  |
   | **B** | 2.24  | 0.00  | 3.16  | 5.00  | 6.32  |
   | **C** | 4.12  | 3.16  | 0.00  | 4.12  | 3.26  |
   | **D** | 7.07  | 5.00  | 4.12  | 0.00  | 5.39  |
   | **E** | 7.00  | 6.32  | 3.26  | 5.39  | 0.00  |

   - **Round 1:** Merge the closest pair A and B into a cluster.
   - **Round 2:** Apply Single Linkage, Average Linkage, and Complete Linkage to determine the next merge. For each linkage method, identify the next cluster merge and explain how the choice of linkage affects the clustering result.

6. Consider a Convolutional Neural Network (CNN) layer that receives an input volume of size 128x65x3 (width x height x depth). If this layer uses 12 filters of size 5x5x3 with a stride of 3 and padding 3.

   - Calculate the output volume size of this layer.
   - The number of parameters in this layer.
