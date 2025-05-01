# Association Rule Mining on NYC Restaurant Inspection Data

This project applies the Apriori algorithm to uncover meaningful association rules from public restaurant inspection data in New York City. Using only focused, high-impact attributes such as borough, cuisine type, violation code, and grade, the system identifies interpretable patterns that can assist public health efforts.

---

## Project Overview

- **Algorithm Used:** Apriori (Agrawal & Srikant, VLDB 1994)
- **Dataset Source:** [NYC Open Data – DOHMH Restaurant Inspection Results](https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/43nn-pn8j/about_data)
- **Final Dataset Size:** 5,000 samples
- **Tech Stack:** Python, CSV processing, CLI

---

## How to Run

```bash
python3 main.py market_basket_dataset_small.csv 0.05 0.6
