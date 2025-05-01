# Association Rule Mining on NYC Restaurant Inspection Data

This project applies the Apriori algorithm to discover meaningful association rules in restaurant inspection data from New York City. Focused on real-world applicability and interpretability, the system helps uncover correlations between public health violations, cuisine types, boroughs, and health grades.

---

## Overview

- **Algorithm Used:** Apriori (Agrawal & Srikant, VLDB 1994)
- **Dataset:** NYC DOHMH Restaurant Inspection Results  
- **Language:** Python  
- **Run Environment:** CLI  
- **Deployment:** Local execution with `.csv` input

---

## How to Run

```bash
python3 main.py market_basket_dataset_small.csv 0.05 0.6
```

- `0.05` → Minimum support (5%)
- `0.6`  → Minimum confidence (60%)

Output is saved in `output.txt`.

---

## Data Cleaning & Transformation

- **Selected Columns:**
  - Borough (BORO)
  - Cuisine Type (CUISINE DESCRIPTION)
  - Grade (GRADE)
  - Violation Code (VIOLATION CODE)

- **Transformation Steps:**
  - Removed low-signal fields (address, coordinates)
  - Cleaned categorical features
  - Transformed rows into baskets for pattern mining

---

## Sample Output

```
[10F, Manhattan] => [A]        Confidence: 85.31%
[Coffee/Tea] => [A]            Confidence: 80.26%
```

These association rules indicate trends between specific boroughs/cuisines and better inspection grades.

---

## Key Insights

- Reduces noise through **targeted feature selection**
- Yields highly interpretable rules for public health analysts
- Offers real-world applicability in **restaurant safety monitoring**

---

## Reflection

This project deepened my understanding of unsupervised learning, support/confidence trade-offs, and real-world data wrangling. Building interpretable models from raw city data was both challenging and rewarding, and gave me experience with transforming structured data into usable business insights.

---

## Project Files

- `main.py` – Apriori implementation
- `transform_to_basket.py` – Preprocessing script
- `market_basket_dataset_small.csv` – Cleaned sample dataset
- `output.txt` – Sample rule output

---

## Dataset Source

**Dataset Source:**  
NYC Open Data – DOHMH Restaurant Inspection Results  
URL: https://data.cityofnewyork.us/Health/Restaurant-Inspection-Results/43nn-pn8j  


---


