# 🎓 Student Dropout Risk Prediction

An Educational Data Science project that uses Machine Learning techniques to identify students at risk of dropout or academic failure through attendance and academic performance indicators.

The goal is to demonstrate how data already available in School Management Systems (SMS/SGE) can be transformed into actionable early-warning insights for educators and administrators.

---

## 🎯 Objective

Develop a predictive model capable of detecting students at risk before dropout occurs, allowing schools to implement timely interventions such as tutoring, mentoring, and personalized academic support.

The project aims to complement educational decision-making, not replace professional judgment.

---

## 🏫 Background

This project was inspired by institutional educational statistics related to:

- 📋 Student attendance
- 📚 Failed subjects
- 👨‍🎓 Grade-level distribution

Using these distributions, a realistic synthetic dataset was generated to demonstrate the potential of predictive analytics in education.

---

## ⚙️ Methodology

### 🧩 1. Dataset Generation


This project does not use real student records.

The dataset is synthetically generated using probability distributions inspired by aggregated educational statistics.

No personally identifiable information (PII) or confidential institutional data are included. A synthetic dataset of 500 students was created using distributions observed in institutional reports:

- Attendance records
- Number of failed subjects
- Grade level

### 🚩 2. Risk Definition

An initial risk rule was defined as:

```python
(attendance_absences >= 20) and (failed_subjects >= 3)
```

Students meeting these conditions are classified as high-risk.

### 🌲 3. Model Training

The project trains:

- 🌲 Random Forest Classifier
- 📈 Logistic Regression (future extension)

Two scenarios are evaluated:

1. Ideal dataset (no noise)
2. Realistic dataset (10% label noise)

### 📊 4. Evaluation

The following metrics are analyzed:

- Accuracy
- Precision
- Recall
- F1 Score
- 📉 ROC Curve
- 🎯 Area Under Curve (AUC)
- 🔍 Feature Importance

---

## 📈 Results

### 🟢 Ideal Model

- Accuracy: 100%
- AUC: 1.00

This represents a theoretical scenario where risk is perfectly defined.

### 🟡 Noisy Model

- Accuracy: ~84%
- Precision (High Risk): ~72%
- AUC: >0.90

Even under realistic uncertainty, the model maintains strong predictive performance.

---

## 🔎 Most Important Features

The model identifies the following predictors as the most relevant:

1. 📋 Attendance absences
2. 📚 Failed subjects
3. 🏫 Grade level

These variables contribute most strongly to identifying students at risk.

---

## 🚀 Potential Educational Applications

A real-world implementation could:

- 🔄 Run automatically every month
- 🤖 Analyze data from the School Management System
- 🚨 Generate early-warning alerts
- 👨‍🏫 Prioritize educational interventions
- 📉 Reduce dropout and repetition rates

---

## 🛠️ Technologies Used

- 🐍 Python
- 🐼 Pandas
- 🔢 NumPy
- 🤖 Scikit-Learn
- 📊 Matplotlib
- 🎨 Seaborn

---

## 📂 Project Structure

```text
.
├── notebooks/
│   └── dropout_risk_prediction.ipynb
├── data/
│   └── synthetic_dataset.csv
├── figures/
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── feature_importance.png
├── README.md
└── requirements.txt
```

---

## 💻 Installation

```bash
git clone https://github.com/YOUR_USERNAME/student-dropout-risk-prediction.git

cd student-dropout-risk-prediction

pip install -r requirements.txt
```

---

## ▶️ Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Then execute the notebook cells sequentially.

---

## 📊 Key Insights

The experiment demonstrates that:

- Educational data already collected by schools can be used for predictive analytics.
- Attendance and academic performance are strong indicators of future risk.
- Machine Learning can support educational decision-making by identifying vulnerable students earlier than traditional methods.

---

## ⚠️ Limitations

This project uses synthetic data generated from aggregated institutional statistics.

Results should be interpreted as a methodological proof of concept rather than a real measurement of student risk.

---

## 🔮 Future Work

- 📡 Integration with real School Management Systems
- 🧠 Explainable AI (SHAP, LIME)
- 📊 Interactive dashboards for school administrators
- 🚨 Automated early-warning notification systems
- 🎯 Individual risk probability monitoring
- ☁️ Web-based deployment

---

## 🤝 Contributing

Contributions, suggestions, and educational collaborations are welcome.

Feel free to open an issue or submit a pull request.

---

## 📜 License

This project is released under the MIT License.

---

### 💡 Educational Impact

> “Data science does not replace teachers' expertise; it enhances it. By identifying students at risk earlier, schools can intervene sooner and provide more effective support.”
