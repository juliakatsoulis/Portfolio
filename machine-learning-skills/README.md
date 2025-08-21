# Machine Learning Skills

This folder contains projects in clustering, optimization, and binary classification. My work highlights both the mathematical foundations and the practical implementation of algorithms, with a focus on interpretability and performance evaluation.


# Files

**binary_classification.ipynb:**

I built and compared Logistic Regression and Linear SVM models in PyTorch to classify handwritten digits from the MNIST dataset (binary 0 vs 1 task). By experimenting with optimization strategies (SGD, Momentum, different learning rates), I achieved ~99.9% accuracy while demonstrating how hyperparameters affect model convergence and stability. 

**optimization.ipynb:**

I implemented and compared gradient descent optimization methods to minimize complex functions and train logistic regression models. By experimenting with different learning rates, momentum, and backtracking line search, I showed how optimization choices affect convergence speed, stability, and accuracy. I also applied these methods on real datasets to demonstrate scalability. 

**tree_clustering.ipynb:**

I used decision trees, K-Means clustering, and random forests to explore supervised and unsupervised learning methods in Python. Using scikit-learn, I trained and tuned a Decision Tree Classifier on a wine dataset with 5-fold cross-validation, achieving ~94% test accuracy, and converted the trained tree into a nested dictionary representation. I also built K-Means from scratch, applied it to customer segmentation data, determined the optimal number of clusters with the elbow method, and interpreted segments such as impulse buyers and luxury buyers. Finally, I trained Random Forest and Logistic Regression models on the ProPublica COMPAS dataset to analyze predictors of recidivism, evaluated feature importance, and discussed algorithmic fairness, showing how age and criminal history dominated predictions while race still had measurable influence.
