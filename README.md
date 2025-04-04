# Predicting Heart Attack Risk with Machine Learning

This project explores the application of supervised learning models to predict heart attack risk based on demographic and medical features.

## 🔍 Objective
Build and evaluate classifiers to estimate heart attack risk using:
- **Non-clinical features** (e.g. age, smoking, BMI)
- **Clinical features** (e.g. blood pressure, cholesterol, ECG)

## 📊 Dataset
- Clean, synthetic-looking dataset with no missing values
- 20+ variables (numeric, binary, categorical)
- Two versions created:
  - **Non-Clinical**: only basic lifestyle/demographic data
  - **Clinical**: includes extended medical parameters

## 🧪 Methods
- Models used:
  - Random Forest
  - K-Nearest Neighbors (KNN)
  - Neural Network (MLP)
  - Frequency Dummy (baseline)
- Metrics:
  - Accuracy
  - Weighted F1-Score
  - F1-Score for Class 3 (high risk)
  - ROC curves

## ⚙️ Pipeline
- Feature Engineering:
  - Ordinal encoding (e.g. Stress_Level)
  - One-Hot encoding (e.g. Gender, ECG_Results)
- Scaling: Min-Max normalization
- Split: 70% train / 15% validation / 15% test
- Tools: Python, scikit-learn

## ❌ Results
None of the models outperformed the dummy baseline.
- Max accuracy: ~50%
- F1 scores: all < 0.40
- ROC curves close to diagonal → random guessing

## 📉 Conclusion
- Models failed due to poor data quality
- No significant patterns detected
- Dataset appears artificially balanced and unrealistic
- No practical predictive value

## ✅ Key Takeaways
- High-quality, real-world data is essential in medical ML
- Even “clean” datasets can be useless if distributions are artificial
- Valuable as a case study in proper ML methodology and evaluation

## 📁 Repository Contents
- `notebooks/`: Python notebooks with full experiments
- `report.pdf`: Full project report (in German)

## 🧠 Author
**Bastian Lipka**  
DHBW Stuttgart  
📧 `wi23004@lehre.dhbw-stuttgart.de`
