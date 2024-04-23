# Bagging

## Learning Goals

- use `sklearn` to build voting models
- describe the algorithm of bagging
- describe the differences among simple bagging, random forest, and extra trees algorithms
- implement bagging models in `sklearn`

## Lecture Materials

[Google Slides: Ensemble Models](https://docs.google.com/presentation/d/1KkH7XixkMg0Kmnm-upzOHmrvEPcGznsGyiwhzJ9n-wo/edit?usp=sharing)
[Jupyter Notebook: Ensembles](ensembles.ipynb)

## Lesson Plan

### Introduction (5 Mins)

Ensemble modeling is a highly effective way of improving model performance, especially inasmuch as it tends to correct for overfitting. There are many varieties, but we'll focus on bagging and boosting.

### Simple and Weighted Averaging ("Voting") (10 Mins)

First, a simple idea for building an ensemble: Just take an average over several different models' predictions.

### Nature of Bagging (20 Mins)

Bagging = Bootstrapping + Aggregating. We'll build multiple models (usually trees), but instead of training each on all data points, we'll train our models via random subsampling of our data points.

### Random Forests (15 Mins)

Over the simple bag, the random forest adds random subsampling of the features as well. This section also illustrates the `.feature_importances_` attribute of the fitted model.

### Extra Trees (5 Mins)

Sometimes a *third* level of randomization is used: Instead of always choosing the optimal branching path, we'll branch randomly.

### Conclusion (5 Mins)

There's a Level Up section on Stacking. The basic idea there is to train a model *on the prediction(s) of other models*. When we get to neural networks in Phase 4, we'll be able to understand these as complex stacks.
