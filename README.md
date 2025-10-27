# 📘 Customer Churn Data Preparation & EDA

## 🎯 Objective
Prepare customer data for modeling using cleaning, feature engineering, and comprehensive exploratory data analysis.

## 🔗 Dataset
**Telecom Customer Churn Dataset** from Kaggle

- Contains customer information, service details, and churn status
- Features include demographics, services subscribed, contract details, and billing information

## 🧠 Key Learning Outcomes
- Handle missing values and inconsistent data types
- Feature engineering (tenure buckets, monthly spend groups)
- Label encoding & correlation analysis
- Advanced visualizations using Seaborn (pairplots, heatmaps, countplots)

## 📋 Project Structure
```
customer-churn-eda/
├── README.md
├── requirements.txt
├── Customer_Churn_Analysis.ipynb   # Main Jupyter notebook
├── archive/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv  # Original dataset
├── data/
│   └── Cleaned_Customer_Churn_Data.csv       # Cleaned dataset output
└── insights/
    └── key_insights.md             # Top 5 insights summary
```

## 🚀 Getting Started

### Prerequisites
```bash
pip install -r requirements.txt
```

### Running the Analysis
1. Download the dataset from Kaggle: [Telecom Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
2. Place `WA_Fn-UseC_-Telco-Customer-Churn.csv` in the `archive/` folder
3. Open and run `Customer_Churn_Analysis.ipynb`

## 📊 Analysis Workflow

### 1. Data Understanding
- Load dataset and examine structure
- Print `.info()` and `.describe()`
- Identify missing or anomalous values

### 2. Data Cleaning
- Fix data types (TotalCharges: object → float)
- Handle missing values (imputation/removal)
- Remove/flag invalid rows

### 3. Feature Engineering
- **TenureGroup**: Categorize tenure (0-12, 13-24, 25-36, 37-48, 49-60, 60+ months)
- **AvgMonthlySpend**: TotalCharges / Tenure
- **MonthlyChargesGroup**: Low (0-35), Medium (35-70), High (70+)
- Convert binary yes/no to 1/0
- One-hot encode categorical variables (Contract, InternetService, etc.)

### 4. EDA & Visualization
- Churn distribution countplot
- Contract type vs Churn barplot
- Correlation heatmap
- Monthly charges by churn status boxplot
- Pairplots for key features
- Additional insights visualizations

## 📈 Key Insights
See `insights/key_insights.md` for detailed findings.

**Quick Summary:**
1. 📊 26.5% overall churn rate indicates retention challenges
2. 📝 Month-to-month contracts show 42% churn vs 11% for two-year contracts
3. ⏰ New customers (0-12 months) are at highest churn risk
4. 🌐 Fiber optic users have higher churn despite premium service
5. 💳 Electronic check payment method correlates with higher churn

## 🛠️ Technologies Used
- **Python 3.8+**
- **Pandas** - Data manipulation
- **NumPy** - Numerical operations
- **Matplotlib & Seaborn** - Visualization
- **Jupyter Notebook** - Interactive analysis

## 📝 Deliverables
✅ Complete Python notebook with documented code  
✅ Top 5 insights summary  
✅ Cleaned CSV file ready for modeling  
✅ Comprehensive visualizations  

## 💡 Actionable Recommendations
1. Incentivize long-term contracts (1-2 year) to reduce churn
2. Focus retention efforts on new customers (first 12 months)
3. Review fiber optic pricing and value proposition
4. Encourage automatic payment methods with incentives
5. Provide additional support/benefits to senior citizens

## 👤 Author
Data Science Project - Customer Churn Analysis

## 📄 License
MIT License

---

**Note:** This project is part of a data science learning curriculum focused on practical EDA skills and customer analytics.
