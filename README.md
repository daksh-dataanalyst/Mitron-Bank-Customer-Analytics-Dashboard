# Mitron Bank — Credit Card Launch: Customer Analytics Dashboard

A data analyst portfolio project analyzing customer demographics, income utilization, and spending behavior for a fictional bank ("Mitron Bank") piloting a new credit card line, built in Excel.

💼 **[LinkedIn Post](#) — link**

---

## Business Problem

Mitron Bank, a legacy financial institution, wants to launch a new line of credit cards. Before committing to a full rollout, their strategy team provided a sample dataset of 4,000 customers across five cities to test whether data-driven analysis could uncover actionable insights to guide the product design.

**My task:** analyze the sample data, identify high-value customer segments, and recommend credit card features backed by the data — then present the findings in a self-explanatory dashboard for a non-technical, executive audience.

## Dataset

Two tables covering 4,000 customers and ~864,000 spend transactions across 6 months (May–October):

| Table | Description |
|---|---|
| `dim_customers.csv` | Customer ID, age group, gender, marital status, city, occupation, average monthly income |
| `fact_spends.csv` | Customer ID, month, spend category, payment type, spend amount |

Cities covered: Mumbai, Delhi NCR, Chennai, Hyderabad, Bengaluru
Occupations covered: Salaried IT Employees, Salaried Other Employees, Business Owners, Freelancers, Government Employees

## Tools Used
- **Microsoft Excel**

## Dashboard Preview

The dashboard has four linked pages, navigable via a custom tab bar, each filterable by age group, occupation, city, gender, marital status, month, and payment type using slicers.


**Demographics**
<br>
<img width="1410" height="860" alt="image" src="https://github.com/user-attachments/assets/d4303ccd-6b59-498e-b6f4-4bc3c4c6cee2" />
<br><br>
**Income Utilization**
<br>
<img width="1407" height="860" alt="image" src="https://github.com/user-attachments/assets/d7ea7f73-d6e1-4829-994b-2b6a9c08a5c8" />
<br><br>
**Spending Behavior**
<br>
<img width="1408" height="862" alt="image" src="https://github.com/user-attachments/assets/fe7ee6ca-7245-4980-95bd-e91b17521583" />
<br><br>
**Executive Summary**
<br>
<img width="1406" height="858" alt="image" src="https://github.com/user-attachments/assets/7a84d415-b8d8-4bed-9e56-6da6c67875c9" />





## Key Insights

**Demographics**
- Sample skews younger and male: 69% of customers are under 35, and the male:female split is 65:35.
- Mumbai is the largest city segment (27%), followed by Chennai (20.9%) and Bengaluru (18.8%).
- Salaried IT Employees are the largest occupation group (32.4% of customers) and also the highest earners.

**Income Utilization (the core metric — avg. spend ÷ avg. income)**
- Overall income utilization is **42.9%**, meaning customers spend under half their income on average across the tracked categories — leaving meaningful room for a credit card to capture additional share of wallet.
- **Salaried IT Employees have the highest income utilization at 50.9%**, despite also having the highest income — this combination of high earning *and* high spend makes them the strongest candidate segment for premium card offerings.
- Government Employees show the lowest utilization (29.0%), suggesting more conservative spending habits relative to income.
- Mumbai customers have the highest income utilization by city (52%), ahead of Delhi NCR (48%) and Bengaluru (44%).

**Spending Behavior**
- **Bills** is the top spend category overall (₹104.9M across the sample), followed by Groceries (₹86.3M) and Electronics (₹79.6M).
- **Credit Card is already the most-used payment method** (41% of transaction value), ahead of UPI (27%), Debit Card (23%), and Net Banking (10%) — indicating existing comfort with card-based payments among this customer base.
- September was the highest average spending month, suggesting a seasonal spike worth investigating further (e.g., festival season spending).

## Data Discrepancies / Assumptions Noted
- A small number of customer records had inconsistent formatting in the `marital status` column header (space instead of underscore) — standardized during cleaning.
- Average income and spend values are treated as monthly figures per the metadata definitions; utilization % is calculated as `avg. monthly spend ÷ avg. monthly income` per customer, then aggregated by segment.
- This is a 4,000-customer *pilot* sample provided by Mitron Bank, not the full customer base — insights should be validated against the full dataset before final rollout decisions.

## Credit Card Feature Recommendations

Based on the segments above, features that align with observed behavior:

1. **Bill-pay rewards / cashback** — Bills is the single largest spend category across all segments; a card offering elevated cashback on utility and bill payments would align with existing habits rather than trying to shift behavior.
2. **Grocery & everyday-spend cashback tier** — Groceries is the #2 category; a rotating or flat cashback on groceries and electronics would appeal broadly, not just to top-tier segments.
3. **Premium tier targeted at Salaried IT Employees** — highest income *and* highest utilization; a card with richer rewards, airport lounge access, or EMI conversion on Electronics could target this segment specifically.
4. **City-specific launch prioritization** — Mumbai's combination of largest customer share and highest income utilization makes it a natural first market for a premium card launch, with Delhi NCR and Bengaluru as strong secondary markets.
5. **UPI-to-credit-card conversion push** — since UPI already holds 27% of transaction value, a card with strong UPI-linked rewards (RuPay credit-card-on-UPI style) could convert existing digital-payment habits into credit card usage rather than competing with them.



**Daksh Jakhar**
