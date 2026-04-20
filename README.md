📘 Megaline Plan Recommendation — Machine Learning Project
📌 Executive Summary
This project focuses on building a machine learning model that recommends one of Megaline’s two mobile plans—Smart or Ultra—based on a subscriber’s monthly usage behavior. The dataset includes call counts, call duration, text messages, and internet traffic for each user.

I evaluated multiple classification models, including Decision Tree, Random Forest, and Logistic Regression, using a structured train/validation/test split. After hyperparameter tuning, the Random Forest model demonstrated the strongest performance and stability. The final model achieved over 0.75 accuracy on the test set, meeting the project requirements and providing a reliable recommendation system.

🗂️ Project Overview
The goal of this project is to classify users into one of two Megaline plans:

Smart (0)

Ultra (1)

Dataset Features
Number of calls

Total call duration (minutes)

Number of text messages

Internet traffic used (MB)

This is a binary classification problem, and the project evaluates multiple models to determine the best-performing approach.

📥 Data Loading & Exploration
I began by loading the dataset and reviewing:

First few rows

Data types

Summary statistics

Missing values

The dataset was clean and ready for modeling without additional preprocessing.

✂️ Train / Validation / Test Split
To ensure fair evaluation:

60% → Training

20% → Validation (for hyperparameter tuning)

20% → Test (final evaluation only)

This split prevents data leakage and ensures unbiased performance measurement.

🤖 Modeling & Hyperparameter Tuning
I trained and compared three models:

1. Decision Tree
Tuned max_depth

Moderate performance, sensitive to depth

2. Random Forest
Tuned n_estimators and max_depth

Most stable and highest accuracy

3. Logistic Regression
Served as a linear baseline

Performed reasonably but limited by linearity

The Random Forest model achieved the best validation accuracy and was selected for final training.

🏁 Final Model Training
The best model was retrained on the combined training + validation data to maximize learning before final testing.

🧪 Test Set Evaluation
The final Random Forest model achieved:

Accuracy ≥ 0.75 (meeting project requirements)

This confirms strong generalization and reliable performance on unseen data.

🧠 Additional Analysis
Confusion Matrix
Used to evaluate class‑level performance and identify misclassification patterns.

Feature Importance
Showed which usage metrics contributed most to the model’s decisions.

📝 Conclusion
This project successfully built a machine learning model capable of recommending Megaline’s mobile plans based on user behavior. The Random Forest model delivered strong performance and met the accuracy threshold. With further enhancements—such as additional features or more advanced algorithms—the model could be improved even further, but it already provides a solid foundation for real‑world use.

🛠️ Technologies Used
Python

Pandas

NumPy

Scikit‑learn

Matplotlib / Seaborn

Jupyter Notebook

🔗 Project Files
megaline_plan_recommendation.ipynb — Full notebook

users_behavior.csv — Dataset

README.md — Project documentation

🙌 Let’s Connect
If you’d like to discuss data analytics, machine learning, or this project, feel free to reach out or connect with me on LinkedIn.
