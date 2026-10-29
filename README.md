Customer Churn Prediction

This project is an end-to-end Machine Learning solution to predict whether a bank customer will churn (exit) based on their demographic and financial data. The project utilizes an Artificial Neural Network (ANN) built with TensorFlow/Keras and features an interactive web interface created with Streamlit.

Features

Data Preprocessing: Handles categorical variables using Label Encoding (for binary features like Gender) and One-Hot Encoding (for multi-class features like Geography). Data is standardized using StandardScaler.

Deep Learning Model: Utilizes a fully connected Artificial Neural Network (ANN) with early stopping and TensorBoard integration for performance monitoring.

Hyperparameter Tuning: Implements scikeras and GridSearchCV to find the optimal number of hidden layers, neurons, and epochs.

Interactive Web App: A user-friendly Streamlit application (app.py) allowing users to input customer data and receive real-time churn probability predictions.

Project Structure

app.py: The main Streamlit application file. Run this to launch the web interface.

Churn_Modelling.csv: The dataset used to train the model (requires download/inclusion in your directory).

model.h5: The trained Keras neural network model.

scaler.pkl: Saved StandardScaler to ensure consistent data scaling during inference.

label_encoder_gender.pkl: Saved LabelEncoder for the 'Gender' feature.

onehot_encoder_geo.pkl: Saved OneHotEncoder for the 'Geography' feature.

Jupyter Notebooks: Contains the step-by-step code for exploratory data analysis, preprocessing, model training, grid search optimization, and inference testing.

Prerequisites

Ensure you have Python 3.8+ installed. The following libraries are required to run the project:

streamlit

pandas

numpy

scikit-learn

tensorflow

scikeras (for hyperparameter tuning notebook)

You can install these dependencies using pip:

pip install streamlit pandas numpy scikit-learn tensorflow scikeras


How to Run the App

Ensure that all the required .pkl files and the model.h5 file are located in the same directory as app.py. If they are not, you will need to run the training notebook first to generate them.

Open your terminal or command prompt.

Navigate to the project directory.

Run the following command:

streamlit run app.py


The application will open in your default web browser. You can now use the sliders and dropdowns to input customer details and evaluate their churn probability.

Usage

In the Streamlit app (app.py), you will be prompted to enter the following customer details:

Geography (France, Germany, Spain)

Gender

Age

Balance

Credit Score

Estimated Salary

Tenure (years with the bank)

Number of Products (bank products used)

Has Credit Card (Yes/No)

Is Active Member (Yes/No)

The app will output the exact probability of the customer churning and provide a final verdict on whether they are likely to leave the bank.
