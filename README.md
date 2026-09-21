# E-Commerce Operations & Logistics Performance Analysis

**Role:** Data Analyst  
**Dataset:** [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## Project Overview

This project analyzes e-commerce fulfillment performance, delivery delays, shipping costs, and customer review ratings using the Brazilian E-Commerce Public Dataset by Olist.

The project integrates order, order-item, product, and review data and creates an analytical dataset for operational performance analysis.

## Business Problem

Late or inefficient fulfillment can affect customer satisfaction and logistics cost. The objective is to identify measurable relationships between delivery performance, customer reviews, and freight cost.

## Objectives

- Integrate multiple Olist CSV datasets.
- Clean delivered-order records and date fields.
- Engineer delivery and logistics metrics.
- Analyze delivery delays and customer review scores.
- Examine freight cost relative to product price.
- Produce business-oriented insights and recommendations.

## Dataset

The original Olist dataset contains approximately 100,000 orders from 2016–2018 and multiple related CSV tables.

**Dataset link:** [Kaggle – Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Project Files

```text
PragyaJain_Olist_Ecommerce_Business_Analytics.ipynb
requirements.txt
PragyaJain_ProjectReport.docx
README.md
```

## Data Processing Workflow

```text
Raw Olist CSV files
        ↓
Data Integration
        ↓
Master Dataset
        ↓
Filtering & Cleaning
        ↓
Feature Engineering
        ↓
KPI Analysis
        ↓
Visualization
        ↓
Business Insights
```

## Verified Results

Using the supplied Olist dataset and the project pipeline:

- **99,441** orders are present in the orders table.
- **96,478** unique orders have status `delivered`.
- The merged item-level master dataset contains **112,650 rows**.
- The final processed analytical table contains **109,316 item-level rows** after cleaning and delivery-duration validation.
- **7.75%** of processed records are associated with delivery after the estimated date.
- Average review score for on-time/early records is **4.21/5**.
- Average review score for delayed records is **2.55/5**.
- **47.02%** of delayed records have a 1-star review.
- **92.25%** of processed records arrive on or before the estimated delivery date.
- Among early records, average earliness is approximately **13.11 days**.
- Records with delivery duration above 30 days have an average review score of approximately **2.23/5**.
- Products under 500g have an average freight-to-price ratio of approximately **41.43%**.

> These results are descriptive associations. They should not be interpreted as proof that delivery time alone causes lower review scores.

## How to Run

1. Download the Olist dataset from Kaggle.
2. Extract the CSV files.
3. Put the required CSV files in the same directory as the notebook.
4. Install dependencies:

```bash
pip install -r requirements.txt
```

5. Open Jupyter Notebook:

```bash
jupyter notebook
```

6. Open `PragyaJain_Olist_Ecommerce_Business_Analytics.ipynb`.
7. Run the notebook cells from top to bottom.

## Key Business Recommendations

- Monitor delayed fulfillment as a high-priority operational KPI.
- Investigate seller, carrier, destination, and product-category patterns behind delays.
- Review estimated delivery dates to improve promise accuracy.
- Examine freight pricing for low-value/lightweight products.
- Track customer review scores alongside delivery performance.

## Source & Attribution

The project uses the Brazilian E-Commerce Public Dataset by Olist, published on Kaggle. The dataset is provided by Olist and is intended for analysis and learning under its stated license.

## Author

**Pragya Jain**
