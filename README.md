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

**Revenue by Gender**
- Male customers contribute 67.74% of total revenue 
  ($157,890) vs Female 32.26% ($75,191)
- Significant gender skew — male segment is 2x 
  the revenue of female segment

**Revenue by Age Group**
- Nearly uniform distribution across all age groups:
  Young Adults (26.66%), Middle-Aged (25.40%), 
  Adult (24.02%), Senior (23.92%)
- Age is not a reliable revenue differentiator 
  in this dataset

**Discount Effectiveness**
- Avg order value without discount: $60.13 (2,223 customers)
- Avg order value with discount: $59.28 (1,677 customers)
- $0.85 difference — discounts have no meaningful 
  impact on purchase amount

**Category Performance**
- Clothing leads transaction volume: 44.54% (1,737 orders)
- Accessories: 31.79% (1,240 orders)
- Footwear: 15.36% (599 orders)
- Outerwear: 8.31% (324 orders)
- Accessories has the highest repeat purchase rate 
  (avg 25.73 previous purchases) despite lower 
  transaction volume than Clothing (25.20)

**Shipping Type vs Customer Satisfaction**
- Standard shipping scores highest (3.82/5.00)
- All shipping types cluster between 3.71–3.82 — 
  difference is minimal (0.11 range)
- Shipping type is not a strong driver of 
  review ratings in this dataset

---

## Business Recommendations

1. **Gender targeting:** Male segment drives 2x revenue —
   prioritize retention and upsell strategies 
   for male customers; investigate why female 
   engagement is lower
2. **Discount strategy:** Blanket discounts show zero 
   ROI on order value — replace with loyalty-based 
   rewards or category-specific promotions
3. **Accessories opportunity:** Highest repeat purchase 
   rate but only 31.79% of transactions — increase 
   Accessories visibility to convert high loyalty 
   into higher revenue share
4. **Age segmentation:** Uniform revenue distribution 
   means age-based campaigns will underperform — 
   shift to behavioral segmentation instead
5. **Shipping investment:** No shipping type meaningfully 
   improves satisfaction scores — avoid over-investing 
   in premium shipping as a satisfaction lever
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
