# ❤️ Heart Disease Prediction System

[![Python](https://img.shields.io/badge/Python-3.12-blue.svg)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Framework-Flask-lightgrey)](https://flask.palletsprojects.com/)
[![scikit-learn](https://img.shields.io/badge/ML%20Library-scikit--learn-yellowgreen)](https://scikit-learn.org/)
[![Model](https://img.shields.io/badge/Model-RandomForestClassifier-brightgreen)](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
[![Status](https://img.shields.io/badge/Status-Deployed-green)]()

---

## 🧠 Project Overview

This Flask-based web application predicts the **10-year risk of heart disease** based on user-input medical information. It uses a **Random Forest Classifier**, trained on the Framingham dataset and scaled with `StandardScaler`.

Users can input health metrics such as cholesterol, blood pressure, smoking status, and more — and get an instant prediction about heart disease risk.

---
## 🔮 Demo WorkFlow
Sample_Workflow[1].png
## 🔮 Demo

📁 **Local Server:** http://localhost:5000

---

## 📊 Model Performance Comparison

| Model                    | ![Accuracy](https://img.shields.io/badge/Accuracy-%3E%3D97%25-brightgreen) | ![F1-Score](https://img.shields.io/badge/F1--Score-0.9729-blue) | ![Precision](https://img.shields.io/badge/Precision-0.9737-purple) | ![Recall](https://img.shields.io/badge/Recall-0.9729-yellow) |
|--------------------------|:------------------------------:|:--------------------:|:----------------------:|:------------------:|
| **RandomForestClassifier** | `0.9729` | `0.9729` | `0.9737` | `0.9729` |
| DecisionTreeClassifier     | `0.9117` | `0.9113` | `0.9240` | `0.9117` |
| XGBClassifier              | `0.9062` | `0.9060` | `0.9121` | `0.9062` |
| KNeighborsClassifier       | `0.7874` | `0.7838` | `0.8125` | `0.7874` |
| GradientBoostingClassifier| `0.7290` | `0.7287` | `0.7313` | `0.7290` |
| SVC                        | `0.6831` | `0.6831` | `0.6837` | `0.6831` |
| LogisticRegression         | `0.6588` | `0.6588` | `0.6591` | `0.6588` |
| AdaBoostClassifier         | `0.6518` | `0.6513` | `0.6543` | `0.6518` |
| GaussianNB                 | `0.5830` | `0.5301` | `0.6356` | `0.5830` |

✅ **Best Model:** `RandomForestClassifier` – delivers the best balance across all metrics.

---

## 🛠️ How to Run Locally

### 1. Clone the Repository

```bash
git clone https://github.com/ShifaZahra123/heart-disease-predictor.git
cd heart-disease-predictor
````

### 2. Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the App

```bash
python app.py
```

Then visit `http://127.0.0.1:5000/` in your browser.

---

## 📁 Project Structure

```
heart-disease-predictor/
│
├── app.py                 # Flask app
├── Models/
│   ├── rf_classifier.pkl  # Trained model
│   └── scaler.pkl         # Scaler for preprocessing
├── templates/
│   └── index.html         # Frontend UI
└── README.md              # This file
```

---

## ✨ Features

* 🧾 User-friendly form for patient data entry
* 💡 Real-time prediction results using ML
* 📊 Clean UI using Bootstrap
* 🔒 Secure form handling

---

## 🙌 Acknowledgements

* [Framingham Heart Study Dataset](https://www.kaggle.com/datasets/aasheesh200/framingham-heart-study-dataset)
* [scikit-learn](https://scikit-learn.org/)
* [Flask](https://flask.palletsprojects.com/)

---

## 📬 Contact

📧 Reach out via GitHub Issues or [shifazahra256@gmail.com](mailto:shifazahra256@gmail.com)
