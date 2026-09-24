# Wells Fargo Checking & Savings Complaint Analysis

## Project Overview

This project analyzes consumer complaints submitted to the Consumer Financial Protection Bureau (CFPB) involving Wells Fargo from January 1, 2022 through December 31, 2025.

The goal is to identify the largest customer pain points, determine which issues are increasing over time, examine how Wells Fargo responds to complaints, and identify opportunities for improvement.

## Business Question

**What are the biggest customer pain points in Wells Fargo checking and savings accounts, and which issues should the company prioritize?**

## Dataset

- **Source:** CFPB Consumer Complaint Database
- **Company:** Wells Fargo & Company
- **Date range:** January 1, 2022 to December 31, 2025
- **Total Wells Fargo complaints analyzed:** 66,193
- **Checking & savings complaints analyzed:** 29,455

The raw CSV is not included in this repository because it is large. The notebook is designed to work with an exported CFPB complaint CSV.

## Tools

- Python
- Pandas
- Matplotlib
- Google Colab
- CFPB Consumer Complaint Database

## Key Findings

### 1. Checking and savings accounts were the largest complaint area in the filtered dataset
The analysis identified **29,455** checking and savings complaints.

### 2. Debit and ATM card complaints increased sharply
Complaints involving problems using a debit or ATM card increased from **758 in 2022** to **1,593 in 2025**, a **110.2% increase**.

### 3. Unauthorized transaction complaints also increased
Unauthorized transaction complaints increased from **495 in 2022** to **1,073 in 2025**, an increase of approximately **116.8%**.

### 4. Response speed does not appear to be the primary issue
Wells Fargo provided a timely response to approximately **99.99%** of checking and savings complaints.

### 5. Monetary relief was meaningful for debit and ATM card issues
Among the major complaint categories examined, debit and ATM card complaints produced the highest number of monetary-relief outcomes.

### 6. Fraud and dispute themes appeared frequently in customer narratives
Exploratory keyword analysis found repeated mentions of:
- disputes and claims
- fraud
- unauthorized activity
- ATM issues
- fees
- refunds and reimbursement

> Note: keyword themes are not mutually exclusive, so one complaint may appear in more than one theme.

## Geographic Findings

California, Florida, and Texas had the highest raw complaint counts in the dataset. These are **complaint volumes, not complaint rates**. State-level counts should not be interpreted as service-quality rankings because population and Wells Fargo customer exposure differ by state.

## Initial Business Recommendation

The findings suggest that Wells Fargo should focus on preventing debit-card and unauthorized-transaction problems before they become complaints.

Potential improvement areas include:

- stronger real-time fraud detection
- proactive transaction alerts
- more granular debit-card controls
- a simpler in-app dispute process
- clearer claim and reimbursement tracking

## Next Phase

The next phase of this project will extend the analysis by:

1. benchmarking Wells Fargo against peer-bank fraud and dispute features
2. identifying evidence-backed operating practices
3. simulating 10%, 20%, and 30% reductions in targeted complaint categories
4. estimating the potential reduction in complaint volume and monetary-relief cases
5. presenting the findings in an executive-style PowerPoint

## Repository Structure

```text
wells-fargo-complaint-analysis/
├── Wells_Fargo_Complaint_Analysis.ipynb
├── README.md
└── .gitignore
```

## How to Run

1. Download a filtered Wells Fargo complaint CSV from the CFPB Consumer Complaint Database.
2. Open `Wells_Fargo_Complaint_Analysis.ipynb` in Google Colab.
3. Run the upload cell and select the CSV.
4. Run the remaining cells from top to bottom.

## Disclaimer

This is an independent portfolio analysis based on public CFPB complaint data. It is not affiliated with or endorsed by Wells Fargo or the CFPB. Complaint data reflects submitted consumer complaints and should not be interpreted as a complete measure of company performance or customer experience.
