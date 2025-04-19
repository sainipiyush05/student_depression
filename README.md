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

You can pass a sample student profile for prediction like this:


sample_input_dict = {
    'Gender': 1,
    'Age': 21,
    'Profession': 2,
    'Academic Pressure': 1,
    'Work Pressure': 2,
    'CGPA': 8.2,
    'Study Satisfaction': 1,
    'Job Satisfaction': 0,
    'Sleep Duration': 6,
    'Dietary Habits': 1,
    'Degree': 0,
    'Have you ever had suicidal thoughts ?': 0,
    'Work/Study Hours': 5,
    'Financial Stress': 1,
    'Family History of Mental Illness': 0
}

sample_input_df = pd.DataFrame([sample_input_dict])
sample_input_df = sample_input_df[X.columns]
sample_input_scaled = scaler.transform(sample_input_df)
pred = final_model.predict(sample_input_scaled)
print("🔮 Predicted Depression:", pred[0])


## 🛠️ Installation

Clone this repository:

```bash
git clone https://github.com/sainipiyush05/student_depression
cd student-depression-prediction


## 📈 Future Work

- Streamlit web app for real-time prediction  
- Feature importance analysis  
- Model explainability using SHAP/LIME  
- Integrate feedback from real students/psychologists  

## 👨‍💻 Author

**Piyush Saini**  
B.Tech CSE | AI/ML Enthusiast  
[LinkedIn](https://www.linkedin.com/in/sainipiyush05) • [GitHub](https://github.com/sainipiyush05)  

## 📜 License

This project is licensed under the **MIT License**.
