# Lecture 3 - Module 1.2 Model evaluation (part 1)

* 

# Notes from Quiz 1 (Lectures 1-3)

### Training vs Prediction Time

* Training time: storing data
  * Usually O(1) or O(n)
* Prediction time: calculate distance between query points (basically the KNN calculation)

### Classification vs Regression

* Classification: goal is to predict  **discrete categories or labels**
  * Examples:
    * Predicting whether an email is spam or not (binary classification).
    * Predicting the weather as "Sunny," "Cloudy," or "Rainy" (multi-class classification).
    * Detecting the type of an animal from an image (e.g., cat, dog, bird).
  * **Output** : A category or label (e.g., Sunny, Cloudy, Rainy in this case).
* Regression: goal is to predict a **continuous value**
  * Examples:
    * Predicting the temperature for tomorrow (e.g., 25.3°C).
    * Predicting house prices (e.g., $450,000).
    * Predicting stock prices or sales revenue.
  * **Output** : A real number (continuous).

### Generalization error

* The generalization error refers to how well a model performs on unseen (test) data. It cannot be reliably approximated by performance on the  **training set** , even if no hyperparameter tuning is performed

  * **Training Error vs. Generalization Error** :
    * The training error reflects how well the model fits the training data.
    * The generalization error reflects the model's ability to perform on new, unseen data.
    * Even without hyperparameter tuning, models can still overfit the training data, causing a discrepancy between training error and generalization error.
  * **Why "No Hyperparameter Tuning" Doesn't Guarantee Generalization** :
    * Even without tuning, the model's architecture and complexity can cause overfitting or underfitting.
    * For example, a highly complex model (e.g., a deep neural network) can perfectly memorize the training set but perform poorly on new data.

### Hyperparameters

* Parameters that are not learned from the data during training but are set before the training process. Examples include:
  * k in **k**-NN.
  * Learning rate in gradient descent.
  * Depth of a decision tree.
  * Number of hidden layers in a neural network.
