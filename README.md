# credit-scoring-logistic

This project focuses on building a credit risk model based on expected loss. 
The main objective is to build a PD (probability of default) model, but later on I also built a LGD (loss given default) and EAD (exposure at default) 
models.

# Methodology
The main objective is to build a PD model with high interpretability.
We do it to preserve the interpretability of the model, since the main user of this model might be non-technical people.
To do so, first we focus on discretizing all variables, using techniques such as coarse and fine classing.
Later on, we build a logistic regression model over such variables.
After that, we compute key metrics to understand the performance of the model, these metrics include Kolmogorov-Smirnov coefficient and Gini coefficient.
Finally, we conclude the PD model by building a table that summarizes key business indicators, such as acceptance rate, fpr, tpr and risk thresholds.
To validate the model, we used the population stability index.
Some secondary objectives were developing both an EAD and LGD models, these models were developed using linear regression and logistic regression.

# Data
Data was extracted from [here](https://www.kaggle.com/datasets/wordsforthewise/lending-club)

# Resources
It is mainly based on [this course](https://www.udemy.com/course/credit-risk-modeling-in-python/)
