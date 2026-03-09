# Customer Churn Dashboard 📊

An interactive Tableau dashboard analyzing customer churn patterns across demographics, geography, and product usage.

---

## Overview

This Tableau workbook (`CustomerChurnDashboard.twbx`) visualizes customer churn data to help identify key drivers of attrition. It includes demographic breakdowns, geographic distribution, and product-level analysis to support retention strategy decisions.

---

## Dashboard Views

| View | Description |
|------|-------------|
| **CustomerChurnDemo** | Main summary dashboard with churn KPIs across Gender, Age, Products, and Map |
| **DetailedTableView** | Granular row-level table for drilling into individual customer records |

### Worksheets

- **Age** — Churn distribution by age group (with adjustable bin size via parameter)
- **Gender** — Churn comparison across gender segments
- **Products** — Churn rate by number of products held
- **Map** — Geographic churn distribution by state
- **Detail** — Supporting detail sheet for the table view
- **Title** — Dashboard title/branding sheet

---

## Data Source

The workbook is built on `customer_churn.csv` — a dataset of bank customers with the following fields:

| Field | Type | Description |
|-------|------|-------------|
| `RowNumber` | Integer | Row identifier |
| `CustomerId` | Integer | Unique customer ID |
| `CreditScore` | Integer | Customer credit score |
| `State` | String | Customer's state |
| `Gender` | String | Customer gender |
| `Age` | Integer | Customer age |
| `Tenure` | Integer | Years as a customer |
| `Balance` | Decimal | Account balance |
| `NumOfProducts` | Integer | Number of bank products held |
| `HasCrCard` | Integer | Credit card ownership (0/1) |
| `IsActiveMember` | Integer | Active membership status (0/1) |
| `Exited` | Integer | Churned flag — 1 = churned, 0 = retained |
| `Complain` | Integer | Complaint flag (0/1) |
| `Satisfaction Score` | Integer | Customer satisfaction rating |
| `Card Type` | String | Type of card held |
| `Point Earned` | Integer | Loyalty points earned |

> **Note:** The data is embedded in the `.twbx` file as a Hyper extract. No external data connection is required to open the workbook.

---

## Requirements

- **Tableau Desktop** or **Tableau Public** (version 2025.3 or later recommended)

---

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Open the workbook**
   - Launch Tableau Desktop or Tableau Public
   - Open `4__CustomerChurnDashboard.twbx`

3. **Explore the dashboards**
   - Start with the **CustomerChurnDemo** tab for a high-level overview
   - Use the **DetailedTableView** tab to drill into specific segments
   - Adjust the **Age Bin Selection** parameter to change age grouping granularity

---

## Parameters

| Parameter | Default | Description |
|-----------|---------|-------------|
| Age Bin Selection | 10 | Controls the width of age buckets in the Age chart |

---

## File Structure

```
.
├── 4__CustomerChurnDashboard.twbx   # Packaged Tableau workbook (includes data)
└── README.md                        # This file
```

---

## License

This project is intended for educational and portfolio purposes. Please ensure you have appropriate rights to any underlying data before sharing publicly.
