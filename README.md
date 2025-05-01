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
