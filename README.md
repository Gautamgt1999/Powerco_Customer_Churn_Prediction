# Powerco_Customer_Churn_Prediction
Instead of aggressive price-cutting—which would thin margins without stopping churn—this analysis recommends that PowerCo focus on loyalty-based retention and high-value customer engagement for clients reaching their 3–5 year tenure mark.
⚡ PowerCo Customer Churn Analysis & Prediction
Business Case: Investigating the impact of price sensitivity on customer retention in the energy sector.

!

Getty Images

📌 Project Overview
PowerCo is experiencing a significant churn rate among its small and medium-sized enterprise (SME) customers. This project analyzes whether price sensitivity is the primary driver of churn and builds a predictive model to identify "at-risk" customers before they leave.

🧪 The Hypothesis
"Is customer churn driven by price increases, or are there deeper operational and tenure-based reasons for customer departure?"

🛠️ Project Pipeline
🔍 1. Exploratory Data Analysis (EDA)
Investigated a dataset of ~14,000 clients to identify patterns.

Key Task: Visualized consumption distributions and price fluctuations.

Findings: Identified significant outliers in energy consumption and skewed price data.

⚙️ 2. Feature Engineering
Transformed raw data into 63+ predictive features.

Temporal Features: Tenure calculation and contract renewal months.

Price Differentials: Calculated the difference between off-peak and peak prices across different months.

Encoding: Transformed categorical sales channels and geographical data into numerical formats.

🤖 3. Predictive Modeling
Deployed a Random Forest Classifier to predict the probability of churn.

Technique: Used Stratified Shuffle Split to handle imbalanced classes.

Metric: Focused on Recall and AUC-ROC to ensure we capture as many potential churners as possible.


Shutterstock
📊 Results & Business Impact
Model Performance
Metric	Score
Accuracy	90.4%
Precision (Churn)	82%
Recall (Churn)	15% (Initial)
💡 Key Strategic Insights
Price Sensitivity is a Weak Driver: Contrary to initial assumptions, price changes are only a minor factor in why customers leave.

Tenure Matters: Customers who have been with PowerCo longer are significantly less likely to churn.

Consumption Volume: Large-scale energy consumers show different churn patterns than low-volume users.

📁 Repository Structure
Bash
├── data/                    # Dataset folder (Client & Price data)
├── EDA.ipynb                # Phase 1: Data Cleaning & Visuals
├── feature_engineering.ipynb # Phase 2: Feature Transformation
├── prediction_modeling.ipynb# Phase 3: ML Model & Evaluation
├── requirements.txt         # Dependency list
└── README.md                # Project documentation
🚀 How to Run
Clone the repo:

Bash
git clone https://github.com/yourusername/powerco-churn-prediction.git
Install requirements:

Bash
pip install -r requirements.txt
Execute Notebooks: Run the notebooks in the order listed in the structure above.
