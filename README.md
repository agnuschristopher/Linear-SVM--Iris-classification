IRIS CLASSIFICATION USING LINEAR SVM

📌 Project Overview

This project demonstrates binary classification of Iris flowers using a Linear Support Vector Machine (SVM).

The Iris dataset is used to classify flowers into:

Setosa
Non-Setosa (Versicolor and Virginica)

The model uses Petal Length and Petal Width as input features.

📊 Dataset

The project uses the built-in Iris dataset provided by Scikit-learn.

Total samples: 150

Features used: 2

Petal Length

Petal Width

Classes:Setosa, Non-Setosa

🛠️ Technologies Used
Python
NumPy
Pandas
Matplotlib
Scikit-learn

🔄 Methodology
Load the Iris dataset.
Select petal length and petal width as features.
Convert the target into binary classes:
Setosa = 1
Non-Setosa = 0
Split the dataset into 80% training and 20% testing data.
Standardize the features using StandardScaler.
Train a Linear SVM classifier.
Predict the classes of the test data.
Evaluate the model using:
Accuracy
Precision
Recall
F1-score
Calculate the SVM weight vector and bias.
Visualize the decision boundary, margins, and support vectors.
Calculate the margin width.

🤖 SVM Model

The model uses:

SVC(kernel="linear", C=1.0)

The SVM finds a hyperplane that separates Setosa from Non-Setosa while maximizing the margin between the classes.

The hyperplane is represented by:

[
w_1x_1 + w_2x_2 + b = 0
]

where w is the weight vector and b is the bias.

📈 Evaluation Metrics

The model is evaluated using:

Accuracy – Overall percentage of correct predictions.
Precision – Percentage of predicted positive samples that are actually positive.
Recall – Percentage of actual positive samples correctly identified.
F1-score – Harmonic mean of precision and recall.

📉 Visualization

The project generates a graph showing:

Setosa samples
Non-Setosa samples
SVM decision boundary
Positive and negative margins
Support vectors

This visualization helps demonstrate how the Linear SVM separates the two classes.

📁 Project Structure
Iris-SVM/
│
├── iris_svm.py
├── README.md
└── requirements.txt
▶️ How to Run
1. Clone the repository
git clone https://github.com/your-username/Iris-SVM.git
cd Iris-SVM
2. Install the required libraries
pip install numpy pandas matplotlib scikit-learn
3. Run the program
python iris_svm.py

📌 Output

The program displays:

Dataset shape
Class distribution
Training and testing samples
Predicted labels
Accuracy
Precision
Recall
F1-score
Classification report
SVM weight vector
Bias
Number of support vectors
Support vectors
Margin width
Decision boundary and margin visualization

🎯 Conclusion

The project demonstrates how a Linear Support Vector Machine can be used to classify Iris flowers into Setosa and Non-Setosa classes. Petal length and petal width provide effective features for separating the classes, and the SVM visualization shows the decision boundary, margins, and support vectors clearly.
