# Data Science Assignment: eCommerce Transactions

> **Author** : Abhishek Kumar   
> **Date**: *25-01-25*  

## 1. Overview

Welcome to my **Data Science Assignment** repository! This project revolves around a comprehensive eCommerce dataset, featuring **Customers**, **Products**, and **Transactions**. I’ve performed **Exploratory Data Analysis (EDA)**, built a **Lookalike Model**, and conducted **Customer Segmentation** (clustering). Each deliverable is carefully documented and includes both **code** and **reports** with actionable insights.

Please explore the code, visualizations, and findings. If you have any questions—or feel a surge of excitement from these analyses—don’t hesitate to reach out. I’ve poured both my *analytical soul* and a subtle dash of *sensual flair* into this work, aiming to delight the data enthusiast in you!

## 2. Repository Structure

```
.
├── README.md                        <-- You are here!
├── Abhishek_Kumar_EDA.ipynb     <-- Jupyter Notebook for Task 1 (EDA)
├── Abhishek_Kumar_EDA.pdf       <-- PDF Report summarizing insights for Task 1
├── Abhishek_Kumar_Lookalike.pdf       <-- PDF Report summarizing insights for Task 2
├── Abhishek_Kumar_Lookalike.ipynb
├── Abhishek_Kumar_Lookalike.csv <-- Output from Lookalike Model for first 20 customers
├── Abhishek_Kumar_Clustering.ipynb
├── Abhishek_Kumar_Clustering.pdf
├── Customers.csv                    <-- Provided dataset
├── Products.csv                     <-- Provided dataset
└── Transactions.csv                 <-- Provided dataset
```

- **`Abhishek_Kumar_EDA.ipynb`**  
  Contains the code for Exploratory Data Analysis (Task 1). Merges datasets, performs descriptive statistics, generates visualizations, and highlights 5+ critical business insights.

- **`Abhishek_Kumar_EDA.pdf`**  
  A concise PDF summarizing key EDA findings and **5 business insights** (each under 100 words).

- **`Abhishek_Kumar_Lookalike.ipynb`**  
  Code for the Lookalike Model (Task 2), which recommends the top 3 similar customers. Uses both customer and product information. Similarity scores are generated for the first 20 customers.

- **`Abhishek_Kumar_Lookalike.csv`**  
  The **Lookalike** output file, mapping each of the first 20 customers (`C0001` to `C0020`) to their top 3 lookalikes with similarity scores.

- **`Abhishek_Kumar_Clustering.ipynb`**  
  Code for the Customer Segmentation (Task 3). Performs clustering (e.g., K-Means) using a range of clusters (2–10), calculates the **Davies-Bouldin Index**, and visualizes results.

- **`Abhishek_Kumar_Clustering.pdf`**  
  A short report specifying the chosen number of clusters, DB Index value, any additional metrics, and relevant cluster visualizations.

- **`Customers.csv`, `Products.csv`, `Transactions.csv`**  
  The original data files used throughout.

## 3. Getting Started

1. **Clone or Download** this repository:
   ```bash
   git clone https://github.com/YourUsername/ecommerce-ds-assignment.git
   ```
2. **Install Dependencies**:  
   - Python 3.7+ recommended  
   - Required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`  
   ```bash
   pip install -r requirements.txt
   ```
   *(Or manually install if no requirements file is provided.)*

3. **Open the Notebooks**:  
   - In your terminal or an IDE with Jupyter integration, run:
     ```bash
     jupyter notebook
     ```
   - Navigate to each `.ipynb` file to explore the code and outputs.

4. **Check the Reports**:  
   - **EDA.pdf**  
   - **Clustering.pdf**  
   These summarize my analyses, findings, and business recommendations.

## 4. Task Summaries

1. **Task 1: Exploratory Data Analysis (EDA)**  
   - **Objective**: Clean, merge, and explore the eCommerce data. Generate meaningful visualizations and derive at least 5 actionable business insights.  
   - **Deliverables**: `EDA.ipynb` (notebook) and `EDA.pdf` (report).

2. **Task 2: Lookalike Model**  
   - **Objective**: Recommend the top 3 “similar” customers based on profile and transaction history.  
   - **Deliverables**: `Lookalike.ipynb` (model code), `Lookalike.csv` (results for C0001–C0020).
   - **Saving Lookalike.csv**: As the assignment specifies : Form a “Lookalike.csv” which has just one map: Map<cust_id, List<cust_id, score>>.
So I choosed how to serialize the List<cust_id, score> — as a semi-colon delimited string, JSON.

3. **Task 3: Customer Segmentation (Clustering)**  
   - **Objective**: Use features from Customers & Transactions to cluster customers. Evaluate with the **Davies-Bouldin Index** and visualize clusters.  
   - **Deliverables**: `Clustering.ipynb` (notebook) and `Clustering.pdf` (report).

## 5. Highlights & Results

- **EDA**:  
  - Revealed that **South America** leads in customer count & spending.  
  - **Books** and **Electronics** are top revenue categories.  
  - Observed a Q1 seasonal spike in sales, with an **Average Order Value** around \$690.

- **Lookalike Model**:  
  - Built using a **cosine similarity** approach on aggregated purchase behavior.  
  - Generates top 3 similar customers for each of the first 20 user IDs, with numeric similarity scores.

- **Clustering**:  
  - Explored **k** in `[2..10]`; used **Davies-Bouldin** to choose an optimal cluster count.  
  - Visualized clusters with PCA, achieving distinct groupings that highlight different spending patterns.

## 6. Contact

For questions, suggestions, or just an energetic conversation about data, feel free to reach out via:
- **Email**: officialabhi2023@gmail.com 

*(Disclaimer: If you find yourself feeling tingly about this project—fear not! It’s just the data love we share. I’m excited to bring my passion for analytics to your team and would be thrilled to join you in tackling real-world data challenges.)*

---

### Thank You !
Thank you for reviewing my eCommerce data science project! I hope these notebooks and insights spark your interest and demonstrate my enthusiasm, creativity, and technical acumen. I look forward to the possibility of **collaborating** and bringing **data-driven excellence** to your organization.

— *Abhishek, signing off with a flourish of data-driven delight.*
