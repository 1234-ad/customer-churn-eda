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
├── churn_analysis.ipynb          # Main Jupyter notebook
├── data/
│   └── cleaned_churn_data.csv    # Cleaned dataset output
└── insights/
    └── key_insights.md           # Top 5 insights summary
```

## 🚀 Getting Started

### Prerequisites
```bash
pip install -r requirements.txt
```

### Running the Analysis
1. Download the dataset from Kaggle: [Telecom Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
2. Place `WA_Fn-UseC_-Telco-Customer-Churn.csv` in the project root
3. Open and run `churn_analysis.ipynb`

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
- **TenureGroup**: Categorize tenure (0-12, 13-24, 25-48, 49+ months)
- **AvgMonthlySpend**: TotalCharges / Tenure
- Convert binary yes/no to 1/0
- One-hot encode categorical variables (Contract, InternetService, etc.)

### 4. EDA & Visualization
- Churn distribution countplot
- Contract type vs Churn barplot
- Correlation heatmap
- Monthly charges by churn status boxplot
- Additional insights visualizations

## 📈 Key Insights
See [insights/key_insights.md](insights/key_insights.md) for detailed findings.

## 🛠️ Technologies Used
- Python 3.8+
- Pandas - Data manipulation
- NumPy - Numerical operations
- Matplotlib & Seaborn - Visualization
- Jupyter Notebook - Interactive analysis

## 📝 Deliverables
✅ Complete Python notebook with documented code  
✅ Top 5 insights summary  
✅ Cleaned CSV file ready for modeling  
✅ Comprehensive visualizations

## 👤 Author
Data Science Project - Customer Churn Analysis

## 📄 License
MIT License
