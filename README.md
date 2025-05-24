# 🏃‍♂️ Running Injury Prediction

This project explores predictive modeling for identifying potential injuries in runners based on physiological, training, and performance-related data. The goal is to assist athletes and coaches in proactively managing training loads to minimize injury risk.

---

## 📊 Project Overview

- **Goal**: Predict the likelihood of a running-related injury using pre-run metrics and historical trends.
- **Data**: Features include weekly mileage, heart rate, sleep quality, soreness levels, and prior injury history.
- **Techniques**: The project applies both exploratory data analysis (EDA) and machine learning modeling techniques to develop a predictive framework.

---

## 📁 Contents

- `running-injury-prediction.ipynb`: Main Jupyter notebook containing EDA, feature engineering, model training, and evaluation.
- `data/`: (Not included) Expected to contain cleaned or raw training datasets such as weekly logs or physiological metrics.

---

## 🧠 Methods

- **EDA Highlights**:
  - Distribution of injury outcomes
  - Correlation analysis between features like weekly mileage, sleep, and injury occurrence
  - Visual trendlines over training periods

- **Feature Engineering**:
  - Lag features for previous week’s soreness and mileage
  - Encoding of categorical indicators like injury history
  - Standardization for numerical inputs

- **Models Used**:
  - Logistic Regression
  - Random Forest Classifier
  - XGBoost (optional)
  
- **Evaluation**:
  - Accuracy, precision, recall, and F1-score
  - Confusion matrix and ROC curves
  - Feature importance analysis

---

## 🚀 Usage

To run the notebook:

```bash
jupyter notebook running-injury-prediction.ipynb
```

Expected data format:
- CSV with rows representing weekly training logs
- Columns such as: `week`, `mileage`, `sleep_hours`, `soreness_score`, `previous_injury`, `injury`

---

## 📦 Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
```

---

## 📈 Example Output

```
Model: Random Forest  
Accuracy: 82.5%  
Precision: 79%  
Recall: 84%  
F1 Score: 81%
```

---

## 🔬 Future Improvements

- Incorporate GPS-derived biomechanical data
- Add time-series RNN/LSTM models
- Personalize predictions using athlete clustering

---

## ⚠️ Disclaimer

This project is for research and educational purposes only. Predictions are not intended to replace medical diagnosis or professional training plans.
