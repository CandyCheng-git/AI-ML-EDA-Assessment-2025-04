# AI-ML-EDA-Assessment-2025-04
**Exploratory Data Analysis (EDA) + baseline ML modelling** — built as a TECH3300 assessment and refactored into a portfolio-ready, reproducible project.

> Recruiter-friendly summary: This repo demonstrates how I take a raw dataset → validate quality → discover insights → build a clean baseline model → evaluate results and limitations.

---

## Quick links
- 📓 Notebook: `TECH3300_Ass1.ipynb`
- 🎨 Slides (Canva): [View my Canva design](https://www.canva.com/design/DAGi5ETvkBE/u6fC7s74jInyWlke8abxWA/view?utm_content=DAGi5ETvkBE&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h19a94a5710)

---

## What this project does
This project follows a practical, end-to-end workflow:
1. **Data audit** (shape, types, missingness, duplicates, outliers)
2. **Exploratory analysis** (univariate + bivariate + target relationships)
3. **Feature preparation** (encoding, scaling, leakage checks, train/test split)
4. **Baseline modelling** (simple models first; complex only if justified)
5. **Evaluation** (right metrics, error analysis, and what I’d do next)

### Why it matters
EDA is where most ML projects succeed or fail. If the data is messy, biased, or leaking target info, “better models” won’t save it.

---

## Dataset
- **Source:** _(add link or citation if public; otherwise say “provided for coursework”)_
- **Rows / Columns:** _(fill in)_
- **Target variable:** _(fill in)_
- **Task type:** _(Regression / Classification)_

> If you can’t publish the dataset, say so clearly and include a small schema/data dictionary.

---

## Key questions answered
Replace these with your actual questions from the notebook:
- What features have the strongest relationship with the target?
- Are there missing values or outliers that distort the model?
- Is the dataset imbalanced (if classification)?
- Which baseline model is “good enough” before optimising?

---

## Method (high level)
### 1) Data quality checks
- Missing values and patterns
- Duplicate rows / inconsistent categories
- Outlier detection (IQR / z-score, depending on column)
- Leakage risk checks (features that directly reveal target)

### 2) EDA
- Distribution plots for numeric features
- Category frequencies for categorical features
- Correlation / association checks (with caution — correlation ≠ causation)
- Target-driven analysis (what actually changes the outcome)

### 3) Baseline model
- Start simple (e.g., Linear/Logistic Regression)
- Add a tree-based model only if it improves *and* stays explainable
- Use cross-validation where appropriate

### 4) Evaluation
- **Regression:** MAE / RMSE / R² + residual checks  
- **Classification:** Accuracy + Precision/Recall/F1 + confusion matrix + ROC-AUC (binary)

_(Keep this section aligned with what your notebook actually does.)_

---

## Results (fill in with your real numbers)
### Model performance
| Model | Metric 1 | Metric 2 | Notes |
|------|----------|----------|------|
| Baseline | _x_ | _y_ | _Short, honest takeaway_ |
| Improved | _x_ | _y_ | _Why it improved_ |

### What I found (insights)
- **Insight 1:** _(e.g., one feature dominates; or missingness is informative)_
- **Insight 2:** _(e.g., strong skew; log transform helps)_
- **Insight 3:** _(e.g., imbalance causes misleading accuracy)_

### Error analysis (what breaks)
- Worst-performing segment(s): _(fill in)_
- Common failure patterns: _(fill in)_
- Suspected causes: _(data sparsity / noise / leakage / bias / small sample)_

---

## How to run (reproducible)
### Option A — Run the notebook (recommended)
1. Create a virtual environment:
   ```
   python -m venv .venv
  ```

2. Activate it:

   * Windows:

     ```bash
     .venv\Scripts\activate
     ```
   * macOS/Linux:

     ```bash
     source .venv/bin/activate
     ```
3. Install dependencies:

   ```bash
   pip install -U pip
   pip install jupyter numpy pandas matplotlib seaborn scikit-learn
   ```
4. Start Jupyter:

   ```bash
   jupyter notebook
   ```
5. Open: `TECH3300_Ass1.ipynb`

> If you already have a `requirements.txt`, replace the install step with:
> `pip install -r requirements.txt`

---

## Repo structure

```
.
├── TECH3300_Ass1.ipynb        # Main notebook (EDA + modelling)
├── README.md                  # You are here
└── (optional) data/           # Raw/processed data (if shareable)
```

---

## Tech stack

* Python (Jupyter)
* pandas / numpy
* matplotlib / seaborn
* scikit-learn

---
