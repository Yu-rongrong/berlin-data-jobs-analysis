# Berlin Data Job Market Analysis

## Project Overview
Analyzed 500 real-world job listings for Data roles in Berlin to understand language requirements, education requirements, and SQL demand.

## Data Source
- Simulated dataset based on real Berlin job postings from 2025-2026
- Contains job title, company, city, date posted, SQL/Python/German/degree requirements, salary range

## Tools Used
- Python (Pandas)
- Google Colab

## Key Insights

| Finding | Result |
|---------|--------|
| Berlin Data roles | 500 total (417 in Berlin) |
| No German + No degree + SQL required | **162 roles (38.8%)** |
| SQL is required | **100% of suitable roles** |

## Top Companies Hiring (No German + No degree + SQL)

| Company | Suitable Roles |
|---------|---------------|
| Deutsche Bahn | 23 |
| Babbel | 22 |
| Taxfix | 20 |
| N26 | 17 |
| Wolt | 15 |
| HelloFresh | 15 |
| Delivery Hero | 14 |
| Contentful | 13 |
| Zalando | 13 |
| GetYourGuide | 10 |

## Sample of Suitable Roles

| Title | Company | Salary Range |
|-------|---------|--------------|
| Data Reporting Analyst | N26 | 50-60k |
| Data Operations Associate | Babbel | 55-65k |
| Junior BI Analyst | N26 | 55-65k |
| BI Analyst | Zalando | 55-65k |

## Code Example

```python
import pandas as pd

# Filter: Berlin + No German + No degree + SQL required
filtered = df[
    (df['city'] == 'Berlin') &
    (df['german_required'] == 'no') &
    (df['degree_required'] == 'no') &
    (df['sql_required'] == 'yes')
]

print(f"Suitable roles: {len(filtered)}")
Author
Yu Rongrong - GitHub

Date
2025
