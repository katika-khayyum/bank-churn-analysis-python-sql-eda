
# 📊 bank-churn-analysis



_👉 End-to-end data analysis and machine learning project to identify key factors driving customer churn and improve retention strategies._

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
## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=alamimran613&theme=radical&no-frame=false&no-bg=false&margin-w=4)


<h2><a class="anchor" id="overview"></a>Overview</h2>

This project performs an end-to-end machine learning pipeline to predict bank customer churn. The goal is to identify customers who are likely to leave the bank, enabling businesses to take proactive action and implement data-driven retention strategies to reduce customer loss.

---

<h2><a class="anchor" id="problem-statement"></a>Problem Statement</h2>

❗ Problem Statement

Customer churn is one of the most critical challenges in the banking industry. Losing a customer is significantly more expensive than retaining one. This project answers the following business question:
- Which customers are most likely to leave the bank, and what are the key factors driving their decision?

By predicting churn in advance, banks can:

- Target at-risk customers with retention offers
- Reduce revenue loss from customer attrition
- Improve overall customer satisfaction and loyalty

---

<h2><a class="anchor" id="dataset"></a>DataSet</h2>

📂 Dataset

Source: Public dataset (GitHub)
- Total Records: 13,500
- Cleaned Records: 10,000+
- Initial Features: 13
- Final Features after Engineering: 20

Target Variable:
- Churn (0 = Not Churned, 1 = Churned)

Class Distribution:
- Not Churned: 7963
- Churned: 2037 (~20%)
---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

🛠️ Tools & Technologies:

- SQL(Common Table Expressions, filtering,groupby)
- Python(Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn)

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

The raw dataset contained 13,500 records with missing values, inconsistencies, and irrelevant columns. The following steps were performed:

Step 1 — Data Cleaning:

- Removed duplicate records and irrelevant columns (RowNumber, CustomerId, Surname)
- Handled missing values and outliers
- Refined 13,500 raw records into 10,000+ clean, usable samples

Step 2 — Feature Engineering:

Expanded features from 13 to 20 variables through new feature creation
Applied the following encoding techniques to handle categorical data

Encoding Techniques Used:

- Label Encoding
- One-Hot Encoding
- Frequency Encoding
- Target Encoding

Step 3 — Class Imbalance Handling:

Detected 80:20 class imbalance (7,963 vs 2,037)
Applied SMOTE (Synthetic Minority Oversampling Technique) to balance classes
After SMOTE: 6,370 samples in each class

Step 4 — Train-Test Split:

80% Training set — 8,000 records
20% Testing set — 2,000 records
Used stratify=y to maintain class distribution in both sets.

---

<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

📊 Exploratory Data Analysis (EDA)

EDA was performed using Matplotlib and Seaborn to uncover patterns and behavioral trends in customer data.

Key visualizations created:

- Churn distribution bar chart
- Age vs Churn distribution
- Balance vs Churn boxplot
- Correlation heatmap of all features
- Active member vs churn rate comparison
- Geography-wise churn analysis
- Product usage vs churn rate
--- 

<h2><a class="anchor" id="key-findings"></a>Key Findings</h2>

🔍 Key Findings:

- 🔴 Inactive account holders showed significantly higher churn rates
- 🔴 Customers with zero balance are more likely to churn
- 🌍 Customers using only 1 product were more likely to churn than multi-product users
- 🟢 Active customers are more loyal and less likely to churn
- Logistic Regression with SMOTE improved churn detection recall from 14% to 72%, making it significantly better at identifying actual churners. Random Forest achieved the highest overall accuracy of 86.45% with strong cross-validation consistency of 81%, confirming robust generalization on unseen data.

---

<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

▶️ How to Run This Project:

1. Clone the repository:
```bash
git clone https://github.com/katika-khayyum/bank-churn-analysis-python-sql-eda.git
```
2. Load the CSVs and into the database:
```bash
cd project:
pip install pandas numpy matplotlib seaborn,imbalanced-learn,scikit-learn
```
- 3.Run the project: python bank_churn_eda.py
---
<h2><a class="anchor" id="author-contact"></a>Author & Contact</h2>

👤 Katika Md Khayyum

- 📧 Email: abdulqhaiyyum0786@gmail.com
- 🔗 [LinkedIn](https://www.linkedin.com/in/katika-md-khayyum-510a6a315/)
