🧠 Customer Churn Prediction & Reward Retention System
This project focuses on identifying potential churners among credit card users using machine learning and proactively reducing churn by offering personalized rewards based on past spending behavior.

🚀 Objective
To predict customer churn using transaction data and implement a retention strategy by:

Clustering customers based on spending behavior.

Predicting churn using a machine learning model.

Offering targeted rewards to high-risk customers based on their historical spending categories.

📊 Dataset
The dataset contains anonymized customer credit card transaction data with features such as:

Balance, purchase frequency, one-off and installment purchases

Cash advances, payment behavior, tenure

A CHURN label indicating whether the customer left or stayed

🧩 Project Modules
1. Clustering (clustering.ipynb)
Goal: Group customers based on their credit card spending behavior.

Method: Applied KMeans clustering on features such as:

BALANCE, PURCHASES, CASH_ADVANCE, TENURE, etc.

Result: Segmented users into different behavioral groups for better reward targeting.

2. Churn Prediction (chrun-prediction.ipynb)
Goal: Predict whether a customer will churn.

Model: Random Forest Classifier

Preprocessing:

Dropped irrelevant or highly missing columns (CUST_ID, MINIMUM_PAYMENTS, etc.)

Scaled and cleaned the data

Accuracy Achieved: ~96%

3. Reward System (reward-system.ipynb)
Goal: Offer rewards to predicted churn customers to encourage retention.

Logic:

Analyze the last spending type (e.g., electronics, groceries, dining)

Match with appropriate offers like:

50–70% off next online purchase

Free grocery item

Buy 1 Get 1 on clothing

30% off dining

Free movie tickets

Result: Personalized retention offers based on real behavior

🧠 Tech Stack
Languages: Python

Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

ML Algorithms: KMeans Clustering, Random Forest

Tools: Jupyter Notebook



🎯 Future Scope
Integrate with a real-time dashboard using Streamlit or Flask

Deploy model for API-based prediction

A/B test reward effectiveness
