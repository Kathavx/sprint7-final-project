# sprint7-final-project   🌐 ** Actual Language:** English | Cambia a: [Español](README.es.md)

# 📊 ConnectaTel — Customer Usage Analysis

Exploratory Data Analysis (EDA) project focused on understanding customer behavior, identifying usage patterns, and developing customer segments to support data-driven business decisions.

---

## 📌 Project Overview

This project analyzes customer information and telecommunications usage data from **ConnectaTel**, with the goal of understanding how customers interact with the company's services.

Through data cleaning, exploratory analysis, statistical summaries, and customer segmentation, the project seeks to identify relevant patterns that can help the business improve its service offerings, strengthen customer retention, and develop more targeted commercial strategies.

## 🎯 Objectives

- Assess the quality and consistency of the available datasets.
- Identify and handle missing values and invalid records.
- Explore customer demographics and service usage patterns.
- Detect and evaluate potential outliers.
- Segment customers by age and usage intensity.
- Translate analytical findings into actionable business recommendations.

## 🗂️ Datasets

The analysis uses three datasets:

| Dataset | Description |
|---|---|
| `users` | Customer information, including age, city, registration date, and subscription details. |
| `plans` | Information about the available telecommunications plans and their features. |
| `usage` | Customer activity records, including calls and text messages. |

## 🛠️ Tools & Technologies

- **Python** — Data analysis and manipulation.
- **Pandas** — Data cleaning, transformation, and aggregation.
- **NumPy** — Numerical operations.
- **Matplotlib** — Data visualization.
- **Seaborn** — Statistical visualizations.
- **Jupyter Notebook** — Interactive analysis and documentation.
- **GitHub** — Version control and project documentation.

## 🔎 Analysis Workflow

The project follows a structured data analysis process:

**1. Data Exploration**
- Inspected dataset dimensions, column types, and general structure.
- Reviewed descriptive statistics and identified initial data quality issues.

**2. Data Cleaning**
- Identified missing and inconsistent values.
- Corrected invalid age values.
- Reviewed registration dates outside the analysis period.
- Evaluated missing values in call and message records.

**3. Data Preparation**
- Converted date columns to appropriate data types.
- Created auxiliary variables to distinguish calls and text messages.
- Aggregated usage information by customer.
- Combined customer and usage information into a consolidated profile.

**4. Exploratory Data Analysis**
- Examined customer age and usage distributions.
- Compared activity patterns across subscription plans.
- Used histograms and boxplots to explore distributions and potential outliers.

**5. Outlier Analysis**
- Identified extreme observations in age, calls, messages, and accumulated call duration.
- Evaluated whether these observations represented errors or potentially meaningful customer behavior.

**6. Customer Segmentation**
- Classified customers into three age groups: Young, Adult, and Older Adult.
- Classified customers into three usage groups: Low, Medium, and High.

**7. Business Insights & Recommendations**
- Interpreted the resulting customer segments.
- Identified potential opportunities for customer retention and service improvement.
- Proposed recommendations for adapting telecommunications plans to customer usage patterns.

## 📈 Key Findings

### Age Segmentation

The customer base was divided into three age groups:

| Segment | Customers | Percentage |
|---|---:|---:|
| Young | 760 | 19.00% |
| Adult | 2,018 | 50.45% |
| Older Adult | 1,222 | 30.55% |
| **Total** | **4,000** | **100%** |

Adults represent the largest customer segment, accounting for approximately half of the customer base.

### Usage Segmentation

Customers were classified according to their call and text message activity:

| Segment | Customers | Percentage |
|---|---:|---:|
| Low Usage | 778 | 19.45% |
| Medium Usage | 2,943 | 73.58% |
| High Usage | 279 | 6.98% |
| **Total** | **4,000** | **100%** |

Medium-usage customers represent the largest segment, while high-usage customers account for a smaller share of the customer base.

### Outlier Analysis

Potential outliers were identified in call and message counts, as well as accumulated call duration.

These observations were retained because there was insufficient evidence to classify them as data entry errors. They may represent legitimate high-activity customers and could provide useful insights for business decisions.

## 💡 Business Recommendations

Based on the analysis, the following opportunities were identified:

- **High-usage customers:** Evaluate plans with higher usage allowances and additional benefits to improve retention.
- **Low-usage customers:** Consider affordable packages and promotional incentives to encourage service engagement.
- **Medium-usage customers:** Maintain competitive plans that meet the needs of the largest customer segment.
- **Customer personalization:** Explore strategies based on demographic characteristics and usage behavior.
- **Usage monitoring:** Track customers with unusually high activity to identify potential opportunities for customer retention and plan optimization.

## 🚀 How to Run the Project

You can reproduce the analysis using Google Colab or Jupyter Notebook.

### Option 1 — Google Colab

1. Download or clone this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload the `.ipynb` notebook.
4. Upload the required CSV datasets.
5. Update file paths if necessary.
6. Run the notebook cells in sequential order.

### Option 2 — Local Environment

Clone the repository:

```bash
git clone <repository-url>
cd <repository-folder>
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook and execute the cells in order.

**Note:** The original CSV datasets must be available in the expected file paths before running the analysis.

## 📁 Suggested Repository Structure

```text
connectatel-customer-analysis/
│
├── data/
│   ├── users.csv
│   ├── plans.csv
│   └── usage.csv
│
├── notebooks/
│   └── connectatel_analysis.ipynb
│
└── README.md
```

## 👨‍💻 Author

**Juan Esteban Ochoa Osorio**

Data Analyst Student | TripleTen Bootcamp

[GitHub Profile](https://github.com/Kathavx)

---

*This project was developed as part of the TripleTen Data Analyst Bootcamp.*
