# ElevateLabs_Task 6

## **Taks 6**:  K-Nearest Neighbors (KNN) Classification

This task focuses on applying KNN Algorithm by measuring the closeness using distance metrics on the given Iris dataset. 
K-Nearest Neighbors (KNN) is a simple and widely-used machine learning algorithm for classification and regression. In classification, KNN works by finding the 'K' closest data points (neighbors) to a new sample and assigning it the most common class label among those neighbors. It doesn’t learn a model during training but instead stores the training data and performs computation during prediction.

## **Dataset**

Iris.csv

## **Tools**

- Python<br>
- Numpy<br>
- Pandas<br>
- Numpy<br>
- Seaborn<br>
- Matplotlib<br>
- Scikit-learn<br>
- Jupyter Notebook<br>

# **Tasks Performed in the dataset**

## 1. Dataset Loading and Preprocessing

In this step, the dataset is loaded using pandas. Here the features and targets are separated into X and y. Feature Normalization is also performed using StandardScalar.

## 2. Data Normalization 

The normalized dataset is then split into training and testing sets using an 80-20 split via train_test_split. This allows the model to be trained on a portion of the data and tested on unseen samples to evaluate performance. PCA transformation is also applied to visualise the decision boundary in 2D.

## 3. KNeighborsClassifier

Using Scikit-learn’s KNeighborsClassifier, a KNN model is trained on the training data. The model is then evaluated with various values of K (from 1 to 10).Then accuracy of the classifier is computed for each K.

## 4. Accuracy and Confusion Matrix

After identifying the best K (the one yielding highest accuracy), the model is retrained using that value. It is evaluated using a confusion matrix to understand how well it predicted each class .

## 5. Visualize decision boundaries

In the final task, to visually understand how KNN separates different classes, the feature space is reduced to two dimensions using Principal Component Analysis (PCA). A custom decision boundary plotting function is used to graphically show the regions each class occupies.
