## 📝 Task 3: Decision Tree Classifier – Summary

**Objective:**  
Build a Decision Tree model to predict whether a customer will purchase a product/service based on demographic and behavioral data (Bank Marketing Dataset).

---

### 🔹 Steps Performed
1. **Data Loading** – Imported dataset (`bank.csv`) using correct delimiter (`sep=';'`).
2. **Exploration** – Checked shape, column info, missing values, and target class distribution.
3. **Cleaning** – Removed extra spaces in categorical data; handled missing values (if any).
4. **Encoding** – Converted target `y` (yes/no) to binary (1/0) and applied one-hot encoding to categorical variables.
5. **Data Splitting** – Split data into 80% train, 20% test sets with stratification.
6. **Model Training** – Trained a baseline `DecisionTreeClassifier`.
7. **Evaluation** – Measured Accuracy, Precision, Recall, F1-score; plotted confusion matrix.
8. **Feature Importance** – Identified top predictors influencing customer purchase.
9. **Hyperparameter Tuning** – Used GridSearchCV to find best tree parameters.

---

### 📊 Key Insights
- **Top Features:** (Replace with your top 3 features from feature importance chart)
- **Best Model Performance:**  
  - Accuracy: `XX%`  
  - Precision: `XX%`  
  - Recall: `XX%`  
  - F1 Score: `XX%`
- Target variable was **imbalanced** (more "no" than "yes"), impacting recall for the minority class.
- Hyperparameter tuning improved model performance compared to baseline.

---

### 🛠 Tools & Libraries
- **Python**  
- **Pandas, NumPy**  
- **Matplotlib, Seaborn**  
- **Scikit-learn**

---

✅ **Conclusion:**  
The Decision Tree model provides an interpretable way to predict customer purchase behavior. However, due to class imbalance, additional techniques like balancing or more complex models (e.g., Random Forest, XGBoost) could further improve performance.

