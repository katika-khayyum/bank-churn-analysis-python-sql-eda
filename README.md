
# 📊 bank-churn-analysis

_👉 Executed end-to-end bank customer churn analysis on 10,000+ records, leveraging feature engineering and advanced visualizations to uncover key drivers and deliver actionable insights for improving customer retention._

---
## 📌 Tables of Content
- <a href="#overview">Overview</a>
- <a href="#problem-statement">Problem Statement</a>
- <a href="#dataset">DataSet</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>
- <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#key-findings">Key Findings</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#author-contact">Author & Contact</a>
---

<h2><a class="anchor" id="overview"></a>Overview</h2>

- This project focuses on analyzing customer churn behavior in a banking dataset. The goal is to identify key    patterns and factors influencing customer attrition using data analysis and visualization techniques.

- The dataset consists of 10,000 customer records, and through feature engineering and encoding, it was expanded to 20 meaningful features for deeper insights.

---

<h2><a class="anchor" id="problem-statement"></a>Problem Statement</h2>

❗ Problem Statement

- Customer churn is a critical problem in the banking sector. Losing customers leads to revenue loss and increased acquisition costs.

Objective:

- Identify customers likely to churn
- Understand behavioral patterns of churned vs retained customers
- Provide actionable insights to reduce churn

---

<h2><a class="anchor" id="dataset"></a>DataSet</h2>
📂 Dataset

- Source: Collected from a public GitHub dataset

- Rows: 10,000
- Initial Columns: 13
- Final Columns after feature engineering: 20

- Key Features:

- Demographics: Age, Gender, Geography
- Financial: Balance, Credit Score, Salary
- Behavioral: Tenure, Active Status, Products
- Target Variable: Churn (0 = No, 1 = Yes)
---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>
🛠️ Tools & Technologies
- SQL(Common Table Expressions, filtering,groupby)
- Python(Pandas, Numpy, Matplotlib, Seaborn, Regular Expressions (re))

---
<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

```
bank-churn-analysis/
├── data/
├── notebooks/
│   ├── bank_churn_eda.ipynb
│   ├── checkpoints.ipynb
├── requirements.txt
├── README.md
├──.gitignore
```
---
<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning & Preparation</h2>

🧹 Data Cleaning & Preparation

- Created a backup of original dataset before preprocessing. 
- Checked and handled missing or inconsistent  values.
- Standardized categorical values (e.g., Gender encoding).

Feature Engineering:

- Created new feature:(Zero Balance → Identifies customers with no account balance).

Derived behavioral insights from:

- Active vs Non-active customers.
- Product usage patterns.

Encoding Techniques Used:

- Label Encoding
- One-Hot Encoding
- Frequency Encoding
- Target Encoding

---

<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>
📊 Exploratory Data Analysis (EDA)

Performed in-depth analysis using advanced visualization techniques:
Univariate Analysis:
- Distribution of Age, Balance, Credit Score
- Churn distribution (imbalanced dataset check)
✔ Bivariate Analysis:
- Churn vs Age, Balance, Activity Status
- Churn vs Geography and Gender
✔ Group-Based Analysis:
- Active vs Churn customers
- Zero balance vs churn
✔ Correlation Analysis:
- Heatmap to identify strong relationships between features
--- 

<h2><a class="anchor" id="key-findings"></a>Key Findings</h2>

🔍 Key Findings:
- 🔴 Inactive members have significantly higher churn rate
- 🔴 Customers with zero balance are more likely to churn
- 🌍 Certain geographic regions show higher churn patterns-
- 🟢 Active customers are more loyal and less likely to churn

---

<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

▶️ How to Run This Project:
1. Clone the repository:
```bash
git clone https://github.com/katika-khayyum/instagram-data-cleaning-python-sql-eda.git
```
2. Load the CSVs and into the database:
```bash
cd project:
pip install pandas numpy matplotlib seaborn
```
- 3.Run the project: python bank_churn_eda.py
---
<h2><a class="anchor" id="author-contact"></a>Author & Contact</h2>

👤 Katika Md Khayyum

- 📧 Email: abdulqhaiyyum0786@gmail.com
- 🔗 [LinkedIn](https://www.linkedin.com/in/katika-md-khayyum-510a6a315/)
