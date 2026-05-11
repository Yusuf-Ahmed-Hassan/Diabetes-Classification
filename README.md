Diabetes Prediction System
Project Description
This project predicts whether a patient has diabetes based on diagnostic measurements. The goal is to build a classification model that can assist in early medical diagnosis by analyzing factors like glucose levels and BMI.

Dataset Information
The dataset consists of several medical predictor variables, such as:

Glucose: Plasma glucose concentration.

BloodPressure: Diastolic blood pressure.

Insulin: 2-Hour serum insulin.

BMI: Body Mass Index.

Age: Patient's age.

DiabetesPedigreeFunction: Genetic influence score.

Target
Outcome: Class variable (0 = No Diabetes, 1 = Diabetes).

Tools Used
Python

Pandas & NumPy

Matplotlib & Seaborn

TensorFlow & Keras

Scikit-Learn

Streamlit (for Deployment)

Data Analysis
Missing Values: Identified and handled "zero" values in columns (Glucose, Blood Pressure, BMI, Insulin) by replacing them with the mean.

Feature Scaling: Applied StandardScaler to normalize inputs, as Neural Networks are sensitive to the scale of features.

Correlations: High correlation was found between Glucose levels and the final Outcome.

Models Used
Neural Network (Multi-Layer Perceptron):

16 neurons in the first hidden layer (ReLU).

8 neurons in the second hidden layer (ReLU).

1 output neuron (Sigmoid).

Optimization: Adam optimizer with Binary Crossentropy loss function.

Results
Training Accuracy: 82.25%

Test Accuracy: 76.62%

The model showed a stable learning curve with 100 epochs and a batch size of 10.

Required Libraries
To run this project, you need to install the following libraries:

Bash
pip install tensorflow pandas numpy scikit-learn seaborn matplotlib streamlit joblib
How to Use
Prepare Files: Ensure app.py, diabetes_model.keras, and scaler.pkl are in the same folder.

Open Terminal: Navigate to the project directory.

Run Application: Execute the following command:

Conclusion
Neural Networks can effectively capture non-linear patterns in medical data.

Data cleaning (handling zero values) was critical for improving the model's predictive power.

The model generalizes well to new data, maintaining a small gap between training and testing performance.
