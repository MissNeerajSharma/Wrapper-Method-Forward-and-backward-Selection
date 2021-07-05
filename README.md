# Wrapper-Method-Forward-and-backward-Selection
What is Feature selection? 
As the name suggests, it is a process of selecting the most significant and relevant features from a vast set of features in the given dataset.

For a dataset with d input features, the feature selection process results in k features such that k &lt; d, where k is the smallest set of significant and relevant features.

So feature selection helps in finding the smallest set of features which results in Training a machine learning algorithm faster. 

Reducing the complexity of a model and making it easier to interpret.
Building a sensible model with better prediction power. 
Reducing overfitting by selecting the right set of features.
Feature selection methods For a dataset with d features, if we apply hit and trial method with all possible combinations of features then total 2^d — 1 models need to be evaluated for a significant set of features.
It is a time-consuming approach, therefore, we use feature selection techniques to find out the smallest set of features more efficiently. 

There are three types of feature selection techniques :

Filter methods
Wrapper methods
Embedded methods 

Difference between Filter, Wrapper and Embedded methods  Filter vs. Wrapper vs. Embedded methods 

In this post, we will only discuss feature selection using Wrapper methods in Python. 

Wrapper methods In wrapper methods, the feature selection process is based on a specific machine learning algorithm that we are trying to fit on a given dataset. It follows a greedy search approach by evaluating all the possible combinations of features against the evaluation criterion. The evaluation criterion is simply the performance measure which depends on the type of problem, for eg. for regression evaluation criterion can be p-values, R-squared, Adjusted R-squared, similarly for classification the evaluation criterion can be accuracy, precision, recall, f1-score, etc. Finally, it selects the combination of features that gives the optimal results for the specified machine learning algorithm.  Flow chart — Wrapper methods Most commonly used techniques under wrapper methods are: Forward selection Backward elimination Bi-directional elimination(Stepwise Selection)
