Forest Cover Type Prediction

Overview

This project aims to classify forest cover types using machine learning models. The dataset used for this project is from the Kaggle competition hosted at Forest Cover Type Prediction. The dataset consists of cartographic variables used to classify forest cover types in Roosevelt National Forest.

Models Used

We experimented with several machine learning models to determine the best approach for this classification task. The models tested include:

k Nearest Neighbors (kNN)

Naive Bayes

Decision Trees

Random Forests

Extra Trees

AdaBoost

Logistic Regression

Stochastic Gradient Descent (SGD)

Support Vector Machines (SVMs)

Gaussian Mixture Models (GMMs)

Best Performing Model

Among all the models tested, AdaBoost combined with Extra Trees yielded the best results. The top-performing models in descending order were:

AdaBoost + Extra Trees

Extra Trees

Random Forests

k Nearest Neighbors

Support Vector Machines

Gaussian Mixture Models

Decision Trees

Models such as Naive Bayes, Logistic Regression, and SGD did not perform well for this problem and were included in the annexes for reference.

Feature Engineering

To further improve the model, we analyzed the existing features and engineered new ones. These engineered features helped enhance the predictive power of the best-performing models.

Ensemble Learning

To achieve better generalization, we ensembled the predictions of the top four models (kNN, AdaBoost, SVMs, and GMMs) by weighting them according to their accuracy.

We excluded Decision Trees, Random Forests, and Extra Trees from the ensemble since they belong to the same family of models as AdaBoost and exhibit similar misclassification patterns. Including them would have overemphasized their mistakes.

Challenges

One key challenge was that the test data distribution was different from the training data distribution. This caused a drop in model performance when making predictions on unseen data. Despite this, our final model achieved 79.51% accuracy on the test set after submission to Kaggle.

Acknowledgments

Kaggle for providing the dataset.

Various online resources and research papers on machine learning and ensemble methods.

Happy coding!

