📋 Project Overview

This project aims to predict whether a person is likely to have a stroke based on health and demographic features.
Using machine learning, I built and compared several classification models to determine the best-performing one for this task.

🧰 Tools & Libraries Used

Python

Pandas, NumPy – Data handling and preprocessing

Scikit-learn – Machine Learning models and evaluation

Imbalanced-learn (SMOTE) – Handling class imbalance

Google Colab – Development environment

⚙️ Data Preprocessing

Loaded the dataset (from Kaggle stroke dataset or similar).

Cleaned the data:

Removed unnecessary columns (like id)

Handled missing values (e.g., in bmi)

⚖️ Handling Imbalanced Data

The dataset had fewer stroke cases compared to non-stroke cases.
To fix this, I applied SMOTE (Synthetic Minority Oversampling Technique) to balance the dataset and improve model fairness.




🧩 Models Tried

I trained and compared the following machine learning models:

Model	Description
Decision Tree	Simple interpretable model, prone to overfitting
Random Forest	Ensemble of decision trees for better generalization
Logistic Regression	Linear model, interpretable and performs well on scaled data
Support Vector Machine (SVM)	Powerful for complex boundaries but slower on large datasets

🔍 Hyperparameter Tuning

I used RandomizedSearchCV to find the best parameters for each model efficiently.

Steps:

Defined a parameter grid for each model.

Used 5-fold cross-validation to evaluate performance.

Selected the best model and parameters based on accuracy and F1-scor

📊 Evaluation Metrics

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

These helped evaluate how well each model handled both classes (stroke and no-stroke).

🧠 Conclusion

✅ Logistic Regression provided the most reliable and interpretable results after scaling and balancing the data.
The combination of StandardScaler, SMOTE, and RandomizedSearchCV helped achieve stable and high-performing results.

👩‍💻 Author

Jana Mohamed
Cairo University – Computer Science
✨ Passionate about AI, Data Science & Machine Learning



Encoded categorical variables using one-hot or label encoding.

Scaled numerical features using StandardScaler to normalize data for better model performance.
