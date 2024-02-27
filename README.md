# Heart Disease Prediction

`Author:` [Kaíque Freire dos Santos]<br>
`Date:` [2024/02/27]

This notebook aims to build machine learning models to predict the presence of heart disease based on patients' clinical data. The dataset used contains information such as age, sex, blood pressure, cholesterol levels, among others.

# Imports

The libraries used in this project are:

* `Pandas:` For data manipulation and analysis.
* `NumPy:` For numeric operations.
* `Matplotlib and Seaborn:` For viewing graphs.
* `Scikit-learn:` For preprocessing, training and evaluating models.
* `XGBoost, Random Forest, SVM, Naive Bayes and MLPClassifier:` Classification algorithms used.

# Loading and Exploratory Analysis

The dataset contains information on 918 patients and 12 attributes, including the presence or absence of heart disease. Initially, the first and last lines of the dataset are displayed, followed by the statistical description and verification of null values.

Additionally, visualizations such as count of heart disease cases, age and cholesterol distribution by heart condition, relationship between cholesterol and blood pressure, and heart disease distribution by sex are presented.

# Preprocessing

Before training the models, the data is pre-processed. Categorical columns are transformed into dummy variables and values are standardized using StandardScaler. Then the data is divided into training and testing sets.

# Machine Learning Models

Models were built using the following algorithms:

* `XGBoost:` A gradient boosting algorithm that uses decision trees.
* `Random Forest:` An ensemble learning algorithm based on decision trees.
* `SVM (Support Vector Machine):` An algorithm that constructs a hyperplane or set of hyperplanes in a high-dimensional space for classification.
* `Naive Bayes:` A classification algorithm based on Bayes' theorem with a naive assumption of independence between features.
* `MLPClassifier:` An artificial neural network with multiple layers of neurons.

For each model, training is carried out using RandomizedSearchCV to find the best hyperparameters. After training, the accuracy, classification report and confusion matrix are presented.

# Conclusion

The models were able to accurately predict the presence of heart disease based on patients' clinical data. XGBoost obtained the highest accuracy among the tested models, followed by Random Forest, SVM, Naive Bayes and MLPClassifier. It is important to highlight that, although the results are promising, clinical interpretation of the models must be carried out by qualified healthcare professionals.

# License

This project is licensed under the MIT License - see the LICENSE file for details.
