# EPSS Data

This repository hosts the **Exploit Prediction Scoring System (EPSS) CSV dataset**, which includes the CVE ID, EPSS score, and percentile for each vulnerability.

## Data

- **File:** `data/epss_scores-2025-11-16.csv`
- **Columns:**
  - `cve`: CVE identifier
  - `epss_score`: EPSS probability score
  - `percentile`: EPSS percentile

## Usage

You can fetch the CSV file directly using the raw GitHub URL:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/<username>/epss-data/main/data/epss_scores.csv"
df = pd.read_csv(url)
print(df.head())
