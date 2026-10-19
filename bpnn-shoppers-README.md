# Predicting Online Shoppers' Purchasing Intention (BPNN)

**Tools:** WEKA, Backpropagation Neural Network (MultiLayerPerceptron), SMOTE | **Context:** ISP560 Machine Learning (UiTM), group project

## Business Question
Which website visitors are going to buy and which are just browsing? Predicting purchase intent in real time lets an e-commerce business focus its effort where it pays off.

## Data
Online Shoppers Purchasing Intention Dataset (Sakar & Kumas, 2018, Kaggle). Target: whether the session ended in revenue.

## Method
1. Loaded and profiled the full dataset in WEKA
2. Normalized attributes so network weights converge
3. Found 84.5% class imbalance and fixed it with the SMOTE filter on the training set
4. Ran 5 BPNN experiments varying hidden layers, learning rate and momentum
5. Applied the enhancement: momentum plus adaptive learning-rate decay

## Results (final model, 20% unseen test partition)
| Metric | Result |
|---|---|
| Accuracy | 88.61% |
| Kappa statistic | 0.5956 |
| Precision (buyer class) | 0.833 |
| Mean absolute error | 0.2133 |

- Page Value was the strongest indicator of revenue-generating sessions
- Kappa and F-measure were reported alongside accuracy because the data was imbalanced

## My Role
I did the preprocessing of the initial data, conducted all the experiments after received feedback for correction from my lecturers. Also, edited the presentation slides and presented the contents clearly.

## Files
- `BPNN ONLINE SHOPPERS PURCHASE INTENTION.pdf` full slides with WEKA screenshots
