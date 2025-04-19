## Student Depression Classification

# 🎓 Student Depression Prediction using Machine Learning

This project uses machine learning models to predict whether a student is suffering from depression based on multiple personal, academic, and social factors.

## 📊 Dataset

The dataset used is `student_depression_dataset.csv`, which includes features such as:

- Age
- Gender
- Profession
- Academic Pressure
- Work Pressure
- CGPA
- Study Satisfaction
- Job Satisfaction
- Sleep Duration
- Dietary Habits
- Degree
- Suicidal Thoughts
- Work/Study Hours
- Financial Stress
- Family History of Mental Illness

The target column is `Depression` (0 = No, 1 = Yes).

## 🧼 Preprocessing

- Dropped unnecessary columns: `id`, `City`
- Encoded categorical features using `LabelEncoder`
- Scaled numerical features using `StandardScaler`
- Train-test split: 80% training, 20% testing

## 🧠 Models Used

We trained and evaluated the following models:

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- AdaBoost

Each model was evaluated on:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC AUC Score

## 🔍 Hyperparameter Tuning

Used `RandomizedSearchCV` for:
- Random Forest
- Support Vector Machine (SVC)
- AdaBoost

Best performing model: **Random Forest**

## 🚀 Model Prediction
🛠️ Installation
Clone this repository:

bash
Copy
Edit
git clone https://github.com/sainipiyush05/student_depression

cd student-depression-prediction

Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run your training or prediction scripts.

📈 Future Work
Streamlit web app for real-time prediction

Feature importance analysis

Model explainability using SHAP/LIME

Integrate feedback from real students/psychologists

👨‍💻 Author
Piyush Saini
B.Tech CSE | AI/ML Enthusiast
LinkedIn | GitHub

📜 License
This project is licensed under the MIT License.

yaml
Copy
Edit

---

Let me know if you'd like:
- `requirements.txt`
- A `Streamlit` version
- A badge-style header (e.g. for accuracy, Python version, etc.)
- To include visuals like confusion matrices or ROC curves in the README
