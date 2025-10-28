# ecommerce-sales-analysis
### 📊 Overview
This project analyzes e-commerce transactions from the **Olist Brazilian E-Commerce Dataset** to uncover sales patterns, customer behavior, and revenue insights using **R** for data cleaning/analysis and **Tableau** for visualization.

### 🧠 Objectives
- Identify top-selling product categories and peak sales months  
- Analyze regional sales distribution across Brazil  
- Compute KPIs: Total Revenue, Orders, and Average Order Value (AOV)  
- Build an interactive Tableau dashboard for stakeholders

### 🧩 Tools Used
- **R** (dplyr, lubridate, ggplot2)  
- **Tableau**  
- **Excel / Google Sheets**  
- **Kaggle Dataset**: [Olist Brazilian E-Commerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

### 📁 Project Structure
ecommerce-sales-analysis/
│
├── data/
│ ├── raw/ # Original Kaggle CSV files
│ └── cleaned/ # Cleaned & merged data exported from R
│
├── scripts/
│ ├── data_cleaning.R # Data import, cleaning, merging
│ ├── exploratory_analysis.R # EDA, trends, and visualizations
│ └── export_for_tableau.R # Final cleaned dataset for Tableau
│
├── tableau_dashboard/
│ ├── dashboard_screenshots/ # PNG screenshots for README
│ └── ecommerce_dashboard.twbx # Tableau workbook
│
└── README.md
### ⚙️ Project Workflow

#### **Step 1: Data Cleaning & Preparation (R)**
- Imported datasets from Kaggle (`orders`, `order_items`, `customers`, `products`, `sellers`).  
- Merged multiple CSVs into one unified dataframe using `dplyr` joins.  
- Handled missing values, removed canceled/unshipped orders, and formatted timestamps using `lubridate`.  
- Created new metrics such as:
  - `order_value = price + freight_value`
  - `order_month`, `order_year`, `delivery_time`

#### **Step 2: Exploratory Data Analysis (EDA)**
- Analyzed sales by month, category, and region.  
- Visualized trends using `ggplot2`.  
- Identified key customer and seller performance metrics.

#### **Step 3: Data Export**
- Saved cleaned dataset as `cleaned_olist_sales.csv` for Tableau integration.

#### **Step 4: Dashboard in Tableau**
- Imported the cleaned CSV and created an **interactive dashboard** featuring:
  - 📈 Monthly Revenue Trend  
  - 🧾 Top Product Categories  
  - 🗺️ Sales by Region (State-level map)  
  - 💳 Payment Type Distribution  
  - 📊 KPI Cards (Revenue, Orders, AOV)

---

### 📈 Dashboard Preview
*(To be added once published on Tableau Public)*  
👉 [View Interactive Dashboard on Tableau Public](#)

You can also find static images in the `/tableau_dashboard/dashboard_screenshots/` folder once added.

---

### 🔍 Insights & Findings
- Electronics and Furniture were the top-performing categories across all years.  
- São Paulo contributed to over 40% of total sales revenue.  
- Sales spiked in Q4 every year, indicating seasonal buying patterns.  
- Average delivery time decreased by 12% in the final year, improving customer satisfaction.  

---

### 🧾 Key Learnings
- Applied **data cleaning and transformation** best practices in R.  
- Strengthened knowledge of **data visualization and dashboard design** in Tableau.  
- Understood how analytics can support real-world **business decision-making**.

---

### 👨‍💻 Author
**Nishanth Kumar Vuppalanchi**  
📧 [nishanth0106@outlook.com](mailto:nishanth0106@outlook.com)  
🔗 [LinkedIn](https://linkedin.com/in/nishanth0106) | [GitHub](https://github.com/Nish010601)

---

### 🪪 License
This project is licensed under the [MIT License](LICENSE).

---

### ⭐ Acknowledgment
Special thanks to **Kaggle** for providing the [Olist Brazilian E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

---

> *“Turning data into insight is the first step in turning insight into action.”*
