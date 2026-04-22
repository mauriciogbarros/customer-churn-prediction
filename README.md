# customer-churn-prediction
A subscription-based company experiences customer churn, which directly impacts revenue.
The goal of this project is to:
1. Identify patterns and drivers of churn
2. Build a model that predicts
3. Translate insights into actioinable business recommendations

### Purpose of this project
This project was developed as a portfolio project to demonstrate:
- Applied data analysis skills
- Machine learning modeling and evaluation
- Clear communication of insights
- Translation of data finding into business value

## 1. Project overview
Customer churn is a major challenge for subscription-based businesses, directly affecting revenue and long-term growth.

This project aims to **analyze, predict, and explain customer churn** using historical customer data and machine learning techniques.

The objectives of this project are:
1. To explore customer behavior and identify patterns associated with churn
2. To build predictive models that estimate churn risk
3. To translate analystical findings into actionable business insights

The project follows and **end-to-end data science workflow**, from data exploration to model interpretation and business recommendations.

### Project structure
customer-churn-prediction/
├── README.md
├── data/
│   └── telco_churn.csv
├── notebooks/
│   └── churn_analysis.ipynb
└── results/
│   └── churn_insights.md
└── requirements.txt


## 2. Dataset description
The analysis uses a **publicly available Telco Customer Churn dataset**, which contains demographic, account, and service-usage information for subscription customers.

### Target variable
- `churn`: indicates whether a customer has left the service (`Yes`/`No`)

### Feature types
- Numerical: tenure, monthly charges, total charges
- Categorical: contract type, payment method, subscribed services

This dataset reflects a realistic business scenario and is suitable for demonstrating applied data science skills.

## 3. Methodology
### 1. Data exploration and cleaning
- Data type validation and missing-value analysis
- Target distribution analysis to assess class imbalance
- Initial statistical summaries

### 2. Exploratory Data Analysis (EDA)
- Churn rates across customer tenure, contract types, and services
- Distribution analysis of numerical features
- Correlation analysis for numerical variables
- Visual insights supported by clear interpretations

### 3. Data processing
- Encoding categorical variables
- Feature scaling
- Train-test with reproducible random seed

### 4. Modeling
Multiple models are trained and evaluated for comparison:
- Logistic regression (baseline model)
- Random forest classifier

### 5. Model interpretation
- Feature importance analysis
- Coeffieicient interpretation (logistic regression)
- Identification of key churn drivers

## 4. Key results
- Customer on **month-to-month contracts** are significantly more likely to churn
- **Short customer tenure** is a strong indicator of churn risk
- Higher monthly charges without long-term commitments are associated with increased churn

Detailed insights and visual explanaations are provided in the analysis notebook and the results summary.

## 5. Business impact
Based on the analysis:
- Encourage long-term contracts through targeted incentives
- Focus retention efforts on high-risk customer segments identified by the model
- Monitor early-tenure customers closely to reduce early churn

A concise summary of recommendations is available in `results/churn_insights.md`

## 6. Technologies used
- python
- pandas, numpy: data handling and numerical computing
- matplotlib, seaborn: visualization
- scikit-learn: machine learning
- Jupyter Notebook

## 6. How to run the notebook
1. Clone the repository
2. Install required python packages
3. Open the notebook `notebooks/churn_analysis.ipynb`
4. Run the cells sequentially to reproduce ethe analysis and results