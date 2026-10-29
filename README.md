# 🏦 Customer Churn Prediction | Deep Learning with ANN

**Predict customer churn. Understand customer behavior. Support smarter banking decisions.**

An end-to-end Machine Learning project that predicts whether a bank customer is likely to leave the bank using demographic and financial information. Built with **TensorFlow, Keras, Scikit-learn, and Streamlit**, this project combines deep learning, hyperparameter optimization, and an interactive web application to deliver real-time churn probability predictions.

## 🚀 Project Highlights

- 🧠 **Deep Learning with ANN** — Predict customer churn using a fully connected Artificial Neural Network.
- 📊 **Data Preprocessing Pipeline** — Handle categorical features, encode variables, and standardize numerical data.
- ⚙️ **Hyperparameter Optimization** — Use `GridSearchCV` and `SciKeras` to explore model architectures and training configurations.
- 🎯 **Churn Probability Prediction** — Estimate the probability that a customer will leave the bank.
- 🌐 **Interactive Web Application** — Enter customer details and receive predictions through a Streamlit interface.
- 📈 **Training Monitoring** — Integrate early stopping and TensorBoard to monitor model training.

## 💡 Why This Project Matters

Customer churn is an important challenge for banks because losing existing customers can affect revenue and long-term customer relationships.

This project uses customer information to estimate churn risk and demonstrate how deep learning can support data-driven decision-making.

**Potential applications:**
- Identify customers who may be at risk of leaving.
- Understand how demographic and financial attributes relate to churn.
- Support targeted customer retention strategies.
- Explore how machine learning models can be deployed through interactive applications.

*Note: Predictions indicate estimated risk, not certainty. Model outputs should be evaluated before being used for real banking decisions.*

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| TensorFlow & Keras | ANN model development |
| Pandas & NumPy | Data manipulation and numerical operations |
| Scikit-learn | Preprocessing, scaling, and model evaluation |
| SciKeras & GridSearchCV | Hyperparameter tuning |
| Streamlit | Interactive web application |
| TensorBoard | Training visualization and monitoring |
| Pickle | Saving preprocessing objects |

## 🧠 Machine Learning Workflow

1. **Data Exploration** — Explore customer demographics, financial attributes, and churn labels.
2. **Data Preprocessing** — Encode categorical features and scale numerical variables.
3. **Model Development** — Build a fully connected ANN using TensorFlow/Keras.
4. **Model Optimization** — Apply grid search to investigate suitable network architectures and training parameters.
5. **Model Persistence** — Save the trained model and preprocessing objects for reuse.
6. **Deployment** — Develop a Streamlit application for interactive predictions.
7. **Inference** — Process new customer inputs using the same preprocessing pipeline and generate churn probabilities.

## 📂 Project Structure

```text
Customer-Churn-Prediction/
│
├── app.py                       # Streamlit web application
├── Churn_Modelling.csv          # Customer churn dataset
├── model.h5                     # Trained ANN model
├── scaler.pkl                   # StandardScaler
├── label_encoder_gender.pkl     # Gender encoder
├── onehot_encoder_geo.pkl       # Geography encoder
│
├── notebooks/
│   ├── data_analysis.ipynb      # EDA and preprocessing
│   ├── model_training.ipynb     # ANN training
│   ├── hyperparameter_tuning.ipynb
│   └── prediction_testing.ipynb
│
├── requirements.txt             # Project dependencies
└── README.md
```

*The notebook names above are illustrative. Adjust them to match the actual files in your repository.*

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd Customer-Churn-Prediction
```

Replace `<your-repository-url>` with your GitHub repository URL.

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

On macOS/Linux:

```bash
source venv/bin/activate
```

### 3. Install dependencies

Create a `requirements.txt` file or install the packages directly:

```bash
pip install streamlit pandas numpy scikit-learn tensorflow scikeras
```

### 4. Prepare the model files

Ensure the trained model and preprocessing files are available in the expected locations. If they are missing, run the model-training notebook to generate them.

The dataset must also be available if the notebooks require it.

### 5. Launch the application

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal to access the application.

## 🖥️ How to Use the Application

Enter the following customer details in the Streamlit interface:

| Input Feature | Description |
|---|---|
| Geography | Customer's country: France, Germany, or Spain |
| Gender | Customer's gender |
| Age | Customer's age |
| Credit Score | Customer's credit score |
| Balance | Bank account balance |
| Estimated Salary | Estimated annual salary |
| Tenure | Number of years with the bank |
| Number of Products | Number of bank products used |
| Has Credit Card | Whether the customer has a credit card |
| Is Active Member | Whether the customer is an active member |

After submitting the details, the application displays the **predicted churn probability** and a corresponding prediction based on the model's decision threshold.

## 📈 Model Evaluation

The project includes an ANN training pipeline and hyperparameter tuning workflow.

To make the evaluation section more informative, report the following metrics after testing the trained model on unseen data:

- **Accuracy** — Overall proportion of correct predictions.
- **Precision** — Proportion of predicted churners who actually churned.
- **Recall** — Proportion of actual churners correctly identified.
- **F1-score** — Balance between precision and recall.
- **ROC-AUC** — Ability to distinguish between churners and non-churners.

*Add your actual evaluation results here after running the model. No performance figures are claimed without measured results.*

## 🔮 Future Improvements

- 📊 Add an interactive dashboard showing churn-risk distributions.
- 📉 Compare ANN performance with Logistic Regression, Random Forest, and XGBoost.
- 🔍 Add explainability using SHAP or feature importance analysis.
- 🎚️ Allow configurable churn-risk thresholds.
- ☁️ Deploy the application to a cloud platform.
- 🧪 Add automated tests for preprocessing and prediction consistency.

## 👨‍💻 Key Learnings

Through this project, I explored:

- Building an end-to-end deep learning pipeline.
- Preparing categorical and numerical data for ANN models.
- Applying hyperparameter tuning to improve model selection.
- Saving and reusing trained models and preprocessing objects.
- Connecting a machine learning model to a user-facing web application.
- Translating model predictions into a practical business use case.

## 🤝 Contributions

Suggestions, bug reports, and improvements are welcome. Feel free to fork the repository and experiment with different models, features, and evaluation techniques.

## 📜 License

Add a license file to specify how others can use, modify, and distribute this project.

---

**Built with Python, Deep Learning, and Streamlit.** 💙

*Exploring how AI can turn customer data into actionable insights.*
