# 🏥 HealthCare Premium Prediction

## 📌 Project Overview

This project is part of the **My Machine Learning Journey**. It predicts **health insurance premiums** based on user attributes such as age, income, BMI category, medical history, and lifestyle habits.

The project uses **machine learning models with segmentation (age-based models)** and provides predictions through an interactive **Streamlit web app**.

---

## 🚀 Features

* 🔮 Predict insurance premium in real-time
* 🧠 Uses **segmented ML models** for better accuracy
* 📊 Handles multiple input features (health + lifestyle)
* ⚙️ End-to-end pipeline (EDA → Training → Deployment)
* 🌐 Interactive UI built using **Streamlit**

---

## 📂 Input Features

The model predicts premium based on:

* Age
* Number of Dependents
* Income (in Lakhs)
* Genetical Risk
* Insurance Plan (Bronze / Silver / Gold)
* Employment Status
* Gender
* Marital Status
* BMI Category
* Smoking Status
* Region
* Medical History

---

## 🧠 Machine Learning Approach

### 🔹 Data Preprocessing

* Handling missing values
* Encoding categorical features
* Feature scaling using **StandardScaler**

### 🔹 Model Strategy

The project uses **segmented modeling**:

| Age Group | Model Used               |
| --------- | ------------------------ |
| ≤ 25      | Linear Regression        |
| > 25      | XGBoost / Advanced Model |

👉 Segmentation improves prediction accuracy by handling different behavior patterns.

---

## 📊 Model Performance

* High accuracy achieved using optimized models
* Better predictions compared to single-model approach
* Important features:

  * Smoking status 🚬
  * Age 👤
  * BMI ⚖️
  * Medical history 🏥

---

## 🛠️ Tech Stack

* Python 🐍
* Pandas, NumPy
* Scikit-learn
* XGBoost
* Joblib
* Streamlit

---

## 📁 Project Structure

```
HealthCare_Premium_Predication/
│
├── artifacts/                # Saved models & scalers
│   ├── model_young.joblib
│   ├── model_rest.joblib
│   ├── scaler_young.joblib
│   └── scaler_rest.joblib
│
├── main.py                   # Streamlit app
├── prediction_helper.py      # Prediction logic
├── requirements.txt
├── README.md
```

---

## ▶️ How to Run

### 1️⃣ Clone Repository

```bash
git clone https://github.com/Farhankhattak078/HealthCare_Premium_Predication.git
cd HealthCare_Premium_Predication
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run App

```bash
streamlit run main.py
```

---

## 💡 Example Prediction

**Input:**

* Age: 30
* Income: 10 Lakhs
* Smoker: Yes
* BMI: Overweight

**Output:**

* Predicted Premium: Higher due to smoking + BMI

