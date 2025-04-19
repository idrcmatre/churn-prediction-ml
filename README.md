# Churn Prediction Using Machine Learning

A supervised learning project to predict customer churn using classic and deep learning models. The dataset includes customer demographics, product holdings, and historical activity. This project demonstrates preprocessing, modeling, evaluation, and comparative analysis.

## 📁 Project Structure

- `data/` – Raw and cleaned datasets used in the project.
- `notebooks/` – Jupyter notebooks for each task:
  - Data Cleaning
  - Decision Tree
  - Logistic Regression
  - Neural Network
  - Final Summary & ROC Comparison
- `visuals/` – All plots used for correlation, performance, validation curves, and final ROC.
- `models/` – Saved model artifacts (.pickle files) for deployment or reuse.

## 🔍 Models Used

- **Decision Tree Classifier**  
  With default and tuned hyperparameters using GridSearchCV

- **Logistic Regression**  
  Tuned for regularization and solver

- **Neural Networks**  
  - Full model with all features
  - Reduced model with top features from decision tree
  - Evaluated using AUC, ROC, Precision, Recall

## 📊 Performance Summary

| Model               | Test Accuracy | F1 (Churn) | AUC Score |
|--------------------|---------------|------------|-----------|
| Decision Tree       | 94.9%         | 0.87       | 0.92      |
| Logistic Regression | 97.4%         | 0.94       | 0.98      |
| Neural Network      | 97.1%         | 0.94       | 0.97      |

## 📌 Tools & Skills Demonstrated

- `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `keras`, `tensorflow`
- Data cleaning, imputation, one-hot encoding
- Feature selection, model comparison, evaluation metrics
- Multi-model analysis with visual performance reporting

## 🧠 Insights

- Logistic Regression and Neural Networks both performed best for the minority class (Churn)
- Dataset imbalance and feature redundancy were addressed through thoughtful preprocessing
- Final ROC curve shows separation between classes across all models

## 🧪 Future Improvements

- Hyperparameter optimization for neural networks using RandomizedSearch
- Integration into a Flask API for serving predictions
- Deployment using Docker or AWS Lambda

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).
