
# 🏥 Health Insurance Premium Predictor

A machine learning web application that predicts a person’s health insurance premium based on lifestyle, medical history, and demographic features. This project demonstrates the end-to-end workflow from data analysis and model building in Jupyter Notebook to deployment using **Streamlit**.

---

## ✨ Features

- Interactive form to collect user input
- Predicts premium using a trained XGBoost regression model
- Streamlit-based responsive UI
- Modular code with a helper module for prediction
- Clean and organised codebase

---

## 🚀 Live App

👉 **https://bharath2903-health-insurance-cost-estimator.streamlit.app/**

---

## 🧠 Technologies Used

- **Python,numpy,pandas**
- **Jupyter Notebook** for EDA and model building
- **XGBoost** for premium prediction
- **Scikit-learn** for preprocessing and model evaluation
- **Streamlit** for web interface
- **Joblib** for model serialization

---

## 🗂️ Project Structure

```
health-insurance-predictor/
├── Jupyter_notebook/
│   ├── data_segmentation.ipynb
│   ├── ml_premium_prediction.ipynb
│   ├── ml_premium_prediction_rest.ipynb
│   ├── ml_premium_prediction_rest_with_scaler.ipynb
│   ├── ml_premium_prediction_young.ipynb
│   └── ml_premium_prediction_young_with_scaler.ipynb
│
├── artifacts/                #joblib files of prediction model
│   ├── model_rest.joblib
│   ├── model_young.joblib
│   ├── scaler_rest.joblib
│   └── scaler_young.joblib
│
├── main.py                   # Streamlit frontend
├── prediction_helper.py      # Model/scaler selection and prediction logic
├── requirements.txt          # Project dependencies
├── README.md                 # Project overview
└── .gitignore

```

---

## 📊 Dataset

> ⚠️ *The dataset used in this project is provided as part of a [CodeBasics](https://codebasics.io) course and is not included in this repository due to licensing restrictions.*

The dataset included 50,000 records with features such as:
- Age
- Gender
- Region
- Marital_status
- Number Of Dependents
- BMI_Category
- Smoking_Status
- Employment_Status
- Income_Level
- Income_Lakhs
- Medical History
- Insurance_Plan
-Annual_Premium_Amount


---

## 📓 Model Development

Model development was done in the [`ml_premium_prediction_rest_with_gr.ipynb`](notebooks/ml_premium_prediction_rest_with_gr.ipynb) notebook and [`ml_premium_prediction_young_with_gr.ipynb`](notebooks/ml_premium_prediction_young_with_gr.ipynb). Key steps included:
- Exploratory Data Analysis (EDA)
- Feature engineering
- Correlation analysis
- Training and comparing different regression models like linear,ridge and  XGBoost regression model.
- Evaluating using metrics like MAE, RMSE
- Error Analysis
- Exporting the final model(XGBoost model) using `joblib`

---

## 🖥️ How to Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/health-insurance-predictor.git
   cd health-insurance-predictor
   ```

2. **Create a virtual environment and activate it**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Streamlit app**
   ```bash
   streamlit run app/main.py
   ```

---

## 📸 Screenshots 

<img width="1468" height="758" alt="image" src="https://github.com/user-attachments/assets/0ba6f8b9-65fc-4c9b-8de1-28cc7f1a2437" />

<img width="1007" height="790" alt="download" src="https://github.com/user-attachments/assets/1ee9cb25-0787-4c20-a318-4f8eb4884bc7" />
<img width="1146" height="700" alt="image" src="https://github.com/user-attachments/assets/0599ae0e-7e1a-4114-b10f-da6f5831d209" />



---

## 🙋‍♂️ Author

- **Bharath Srinivas**
- [LinkedIn](https://www.linkedin.com/in/bharath-srinivas-286460344/) • [GitHub](https://github.com/bharath2903)

> Project built as part of the CodeBasics ML course.
