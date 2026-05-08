# Customer Shopping Behavior Analysis

End-to-end analytics project on 3,900+ customer records 
to identify revenue drivers, spending patterns, and 
customer segments — from raw data to actionable dashboard.

**Stack:** Python · PostgreSQL · Power BI

---

## Business Problem

Retail businesses collect transaction data but rarely 
extract structured insight from it. This project answers:

- Which customer segments generate the most revenue?
- Do discounts actually increase spending?
- Which product categories drive consistent engagement?
- How does age and gender affect purchase behavior?

---

## Dataset

- 3,900+ records across 18 features
- Includes: customer demographics, purchase amount, 
  product category, discount usage, shipping type, 
  review ratings, subscription status

---

## Workflow

### 1. Data Cleaning & EDA (Python)
- Handled missing values and standardized column names
- Feature engineering: age group buckets, 
  purchase frequency tiers
- EDA: distribution analysis, correlation checks, 
  outlier detection
- Exported cleaned data to PostgreSQL

### 2. SQL Analysis (PostgreSQL)
Key queries built:
- Revenue segmentation by gender and age group
- High-spending discount users vs non-discount users
- Top-rated products by category
- Shipping type vs delivery satisfaction correlation
- Customer loyalty segmentation (RFM-style)

### 3. Dashboard (Power BI)
- KPIs: Total Revenue, Avg Order Value, 
  Customer Count by Segment
- Slicers: Category, Gender, Age Group, Season
- Visuals: Revenue trends, segment breakdown, 
  product performance

---

## Key Findings

- Customers aged 25–34 contribute ~38% of total revenue 
  despite being 27% of the dataset
- Discount users do not spend significantly more — 
  average order value difference is under 4%
- Clothing and accessories drive 60%+ of repeat purchases
- Free shipping correlates with higher review ratings 
  across all categories

---

## Business Recommendations

1. Focus retention budget on 25–34 age segment — 
   highest ROI per customer
2. Reduce blanket discounting — data shows minimal 
   impact on order value
3. Prioritize free shipping offers for clothing category 
   to improve satisfaction scores

---

## Repository Structure
├── Data/               # Raw and cleaned datasets
├── Notebook/           # Python EDA and cleaning
├── Sql/                # PostgreSQL queries
├── Dashboard/          # Power BI .pbix file
├── Report/             # Final analysis report
├── Presentation/       # Project slides
└── Problem Statement/  # Original problem definition

---

## How to Run

1. Clone the repository
2. Install dependencies:
   pip install pandas numpy psycopg2

3. Run the notebook in `/Notebook` for EDA
4. Execute SQL scripts in `/Sql` using PostgreSQL
5. Open `.pbix` file in Power BI Desktop

---

## Dashboard Preview

<img width="1437" height="787" alt="Screenshot 2026-05-03 135529" src="https://github.com/user-attachments/assets/68e797be-bf81-42b9-a139-4b5b2ea665ab" />
