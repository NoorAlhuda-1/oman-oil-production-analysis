# Oman Oil Production: Trend Analysis and Forecast Test

Analysis of crude oil production for Oman and Gulf producers using the
Energy Institute Statistical Review of World Energy dataset (1965-2025).

## What I did
- Cleaned and reshaped the Excel data in Python (pandas)
- Queried it with SQL (SQLite): Oman's 10-year production, Gulf comparison
- Tested a linear trend model against simple baselines on held-out years (2023-2025)

## Findings
- Oman produced about 995 thousand barrels/day on average in 2016-2025
  (range 951-1,064), the smallest producer among the Gulf countries compared.
- A simple 2016-2022 average (MAE 27 kbd) beat a linear trend (MAE 39)
  and a last-value baseline (MAE 50).
- Oman's output looks stable within a range rather than growing.

## Limitations
- The test set is only 3 years, so conclusions are tentative.
- The model uses past production only; it ignores OPEC+ quotas, prices and field decline.

## Tools
Python, pandas, scikit-learn, matplotlib, SQL (SQLite), Google Colab
