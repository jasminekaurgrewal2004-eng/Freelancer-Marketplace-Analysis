# Project Insights Report

This report summarizes high-level metrics from the current cleaned datasets.

## 1) Dataset Coverage

### Raw vs Clean Row Counts

| Dataset | Raw Rows | Clean Rows |
|---|---:|---:|
| Freelancers | 507 | 488 |
| Projects | 1200 | 500 |
| Reviews | 2874 | 3500 |
| Transactions | 3500 | 3500 |

## 2) Transactions Overview (`clean_transactions.csv`)

- Date range: `2020-01-01` to `2024-12-31`
- Total GMV: `$67,450,975`
- Average transaction amount: `$20,050.82`
- Median transaction amount: `$3,948`
- Average platform fee: `13.10%`
- Success rate: `51.23%`
- Dispute rate: `49.11%`

Interpretation:
- The gap between mean and median suggests a strong right-skew with large outliers.
- Dispute rate is unusually high and should be validated against business definitions.

### Top Payment Methods (count)

1. Crypto: 575
2. Wise: 553
3. PayPal: 553
4. Stripe: 528
5. Bank Transfer: 526

### Top Freelancers by Total Transaction Volume

| Freelancer ID | Total Amount (USD) |
|---|---:|
| FL00174 | 1,696,409 |
| FL00486 | 1,531,095 |
| FL00305 | 1,422,413 |
| FL00153 | 1,217,391 |
| FL00184 | 1,083,785 |

## 3) Freelancer Profile Overview (`clean_freelancer.csv`)

- Verified profiles: `45.70%`
- Profile completion rate: `58.20%`
- Average hourly rate: `$60.74`
- Median hourly rate: `$50.00`
- Average rating: `4.00`
- Average experience: `7.34 years`

### Most Common Skills

1. wordpress (37)
2. react (37)
3. copywriting (35)
4. php (35)
5. flutter (34)
6. seo (34)
7. graphic design (32)
8. devops (32)

## 4) Missing Data Snapshot (Clean Files)

- `clean_freelancer.csv`: `primary_skill` (3.89%), `email` (3.48%), `country` (3.07%), `join_date` (2.46%), `name` (1.02%)
- `clean_projects.csv`: `primary_skill` (3.80%), `email` (3.60%), `country` (3.00%), `join_date` (2.40%), `name` (1.00%)
- `clean_reviews.csv`: `platform_fee_pct` (5.40%), `payment_date` (5.03%), `freelancer_id` (4.83%), `project_id` (4.20%), `payment_method` (4.06%), `amount` (3.89%), `currency` (2.89%)
- `clean_transactions.csv`: same null pattern as `clean_reviews.csv`

