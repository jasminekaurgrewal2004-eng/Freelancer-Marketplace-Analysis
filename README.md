# Freelancer Marketplace Data Cleaning and Insights

This project contains raw and cleaned datasets for a freelancer marketplace-style platform, along with exploratory cleaning work in a Jupyter notebook.

## Project Contents

- `freelancers.csv` -> raw freelancer profiles
- `projects.csv` -> raw project records
- `reviews.csv` -> raw client review records
- `transactions.csv` -> raw payment transactions
- `clean_freelancer.csv` -> cleaned freelancer dataset
- `clean_projects.csv` -> cleaned projects dataset
- `clean_reviews.csv` -> cleaned reviews dataset
- `clean_transactions.csv` -> cleaned transactions dataset
- `dataset_cleaning.ipynb` -> notebook used for cleaning and transformations
- `INSIGHTS.md` -> key metrics and data quality observations

## Quick Snapshot

- Raw rows: freelancers `507`, projects `1200`, reviews `2874`, transactions `3500`
- Clean rows: freelancers `488`, projects `500`, reviews `3500`, transactions `3500`
- Transaction success rate: `51.23%`
- Dispute rate: `49.11%`
- Total transaction volume (GMV): `$67,450,975`

## Main Insights

See full details in `INSIGHTS.md`.

Highlights:
- Transaction values are highly skewed (`mean $20,050.82` vs `median $3,948`).
- Average platform fee is `13.10%`.
- Verified freelancers represent `45.70%` of cleaned freelancer profiles.
- Most frequent skills include `wordpress`, `react`, `copywriting`, and `php`.

## Data Quality Notes

- `clean_projects.csv` appears to contain freelancer-like schema instead of project-specific fields.
- `clean_reviews.csv` appears to contain transaction-like schema instead of review-specific fields.
- Missing values are still present in cleaned files (for example `platform_fee_pct`, `payment_date`, and identifier fields in transaction/review datasets).

## Power BI Dashboard image:
<img width="911" height="513" alt="image" src="https://github.com/user-attachments/assets/2f4e4cf3-6411-4914-9d4c-b2e4de7e7fef" />


