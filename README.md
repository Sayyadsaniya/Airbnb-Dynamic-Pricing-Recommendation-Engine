# Airbnb-Dynamic-Pricing-Recommendation-Engine

Initial Dataset Overview (AB_US_2023.csv)
Total Rows: 232,147

Total Columns: 18

Key Data Issues Identified:
Missing Values:

name: 16 missing

host_name: 13 missing

neighbourhood_group: ~135K missing (~58%)

last_review & reviews_per_month: ~49K missing (likely related to properties with no reviews)

Data Types Warning:

Column 4 (neighbourhood_group) shows mixed types—needs consistent formatting or imputation.

Outliers / Inconsistent Values:

price ranges from 0 to 100,000 USD – requires capping or flagging.

minimum_nights maxes out at 1250 nights – needs validation.

Redundant / Low-value Columns:

id, host_id are likely identifiers only.



Cleaned Dataset Summary: Download Cleaned CSV
Total Rows: 231,790

Total Columns: 18

Columns with Missing Values: Only last_review has 48,884 missing (no reviews).

Key Data Improvements:
Dropped rows with missing essential identifiers (name, host_name).

Filled neighbourhood_group with "Unknown".

Capped extreme values for price (max 10,000 USD) and minimum_nights (max 365).

Filled missing reviews_per_month with 0.

Converted last_review to datetime.

Overview:
Price Range: $1 – $10,000

Minimum Nights: 1 – 365

Room Types:

Entire home/apt: 169,038

Private room: 59,586

Shared room: 2,273

Hotel room: 893

Top Cities:

New York City: 42,863

Los Angeles: 42,377

Broward County: 16,887

Austin: 14,351

Clark County: 13,843





