## Repo contains

**GreenVi$or: Transparent Decision Support for Sustainable Microfinance Lending**

**Author:** Sumaiya Rahman (Student No. 25011484)  
**Supervisor:** Dr. James Barrett  
**Programme:** MSc Data Science, University of the West of England (UWE)  
**Submission:** January 2026

**Files included in this repository (main):**
- `01_clean_features.py` (cleaning + feature engineering)
- `02_train_models.py` (Logistic Regression + Random Forest)
- `03_shap_explain.py` (SHAP explainability)
- `04_impact_dials.py` (Environmental / Social / Circularity scoring)
- `05_decision_rules.py` (Fund / Review / Reject rules)
- `streamlit_app.py` (basic visual prototype, opt)
- `Greenvisor_Report.pdf` (submitted dissertation)
  
---

## Data access and acknowledgement
This project uses Kiva historical snapshot loan data.  
Data Link: (https://www.kiva.org/build/data-snapshots)

(note: Raw Kiva snapshot files are not included in this repository due to data access and redistribution constraints.  
Only derived and cleaned outputs are generated locally.)


---

## Models implemented

- Logistic Regression (baseline)
- Random Forest (comparative)

Target label: **Funded vs Expired (viability classification)**  
Metrics: ROC-AUC, Precision, Recall, F1, Calibration.

---

## Impact scoring

Three transparent proxy-based impact dials are implemented:

- Environmental  
- Social  
- Circularity  

Scoring is based on policy-anchored proxy tables (DEFRA / WRAP / Social Value Model).

---

## How to reproduce

1. Install Python packages (once):
   pip install -r requirements.txt
   
3. Download Kiva snapshot data and place CSV files in:
   data/raw/
   
5. Run scripts in order:
python 01_clean_features.py
python 02_train_models.py
python 03_shap_explain.py
python 04_impact_dials.py
python 05_decision_rules.py

---

Outputs will be saved in:
data/processed/
figures/
results/

---

## License and academic use

This repository is provided for academic assessment and research purposes only.  
Kiva data remain subject to Kiva’s data usage policy and must not be redistributed.

---

## Contact

Sumaiya Rahman  
MSc Data Science - University of the West of England  
Student ID: 25011484  
sumaiya2.rahman@live.uwe.ac.uk


