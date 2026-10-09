# OIBSIP — Oasis Infobyte Data Science Internship

**Intern:** Aphile Ashley  
**Track:** Data Science  
**Internship commence date:** 5 October 2026  
**Final submission deadline (offer letter):** 15 November 2026  
**Repository:** this public repository, named exactly `OIBSIP`

> This repository contains my work for the Oasis Infobyte (OIBSIP) Data Science internship. The task list requires **at least 3 of 5** Data Science tasks; I am attempting Tasks 1, 2 and 5.

## Tasks

| # | Task | Folder | Status |
|---|------|--------|--------|
| 1 | Iris Flower Classification | [DataScience-Task1-IrisFlowerClassification](DataScience-Task1-IrisFlowerClassification/) | **In progress — setup, data inspection, and visualizations verified; interpretation pending** |
| 2 | Unemployment Analysis with Python | [DataScience-Task2-UnemploymentAnalysis](DataScience-Task2-UnemploymentAnalysis/) | Not started |
| 5 | Sales Prediction Using Python | [DataScience-Task5-SalesPrediction](DataScience-Task5-SalesPrediction/) | Not started |

**Task 1 progress so far:** The Iris loading and data-inspection cells have been run. The reported DataFrame has 150 rows and 6 columns; its four measurements are `float64`, `target` is `int64`, `species` is categorical, null counts are zero, and each species has 50 rows. The notebook kernel was verified to use the project `.venv`. The exploratory visualizations have now been generated from the real data: a species-coloured pair plot and four per-feature box plots (saved to the task's `figures/` folder). The plotted frame uses only the four measurement columns plus `species` — the numeric `target` was not included. Written interpretation of the charts, model training, and evaluation are **not yet complete**.

Each task folder contains:

- `AphileAshley_TaskN.ipynb` — the Jupyter notebook for the task
- `README.md` — objective, dataset/source, tools, how to run, methods, findings, and limitations
- `data/README.md` — where to place the real dataset file (Tasks 2 and 5)

## Project setup

```bash
# 1. Clone the repository
git clone https://github.com/DemainMan/OIBSIP.git
cd OIBSIP

# 2. Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch Jupyter from the repository root
jupyter notebook
```

Then open the task notebook you want to review and run it top to bottom.

## Repository files

- [STUDY_NOTES.md](STUDY_NOTES.md) — notes on concepts learned during the internship
- [PRACTICE_EXERCISES.md](PRACTICE_EXERCISES.md) — extra practice problems
- [requirements.txt](requirements.txt) — Python dependencies
- [.gitignore](.gitignore) — keeps `.venv`, caches, checkpoints, and IDE files out of Git

## Submission checklist (all items open until I confirm them)

### Repository

- [ ] Repository is named exactly `OIBSIP` (all capitals)
- [ ] Repository is public
- [ ] Root `README.md`, `requirements.txt`, and `.gitignore` are present and accurate
- [ ] Three task folders use the exact required folder names
- [ ] Notebooks follow the `YourName_TaskNumber` naming rule
- [ ] No credentials, `.venv`, `__pycache__`, or notebook checkpoints are in Git

### Task 1 — Iris Flower Classification

- [ ] Notebook runs end to end from a fresh kernel after all task sections are complete
- [ ] EDA charts, train/test split, at least two classifiers, and full evaluation are complete
- [ ] My written interpretation of charts and model comparison is complete
- [ ] Task `README.md` has my actual findings and limitations
- [ ] Relevant screenshots/output files are saved

### Task 2 — Unemployment Analysis

- [ ] Real “Unemployment in India” CSV obtained from its real source (not invented data)
- [ ] Notebook runs end to end from a fresh kernel
- [ ] Cleaning, regional/monthly analysis, heatmap, and pre/post-COVID comparison with a confirmed cutoff are complete
- [ ] Written observation after every chart; no causal claims
- [ ] Task `README.md` has my actual findings and limitations
- [ ] Relevant screenshots/output files are saved

### Task 5 — Sales Prediction

- [ ] Real `Advertising.csv` obtained from its real source (not invented data)
- [ ] Notebook runs end to end from a fresh kernel
- [ ] EDA, two regressors, MAE/RMSE/R² comparison, residual plot, and coefficient/importance discussion are complete
- [ ] Written interpretation does not present predictive importance as causation
- [ ] Task `README.md` has my actual findings and limitations
- [ ] Relevant screenshots/output files are saved

### Demo videos (one per task, per the task-list workflow)

- [ ] Task 1 demo recorded — first 2 seconds show a static title card with full name, Data Science track, and task title; then show the work running end to end
- [ ] Task 2 demo recorded (same title-card rule)
- [ ] Task 5 demo recorded (same title-card rule)
- [ ] Videos uploaded and links recorded here

### LinkedIn / cohort engagement (per the task-list workflow)

- [ ] Task 1 demo posted on LinkedIn, Oasis Infobyte tagged, and `#oasisinfobyte` included
- [ ] Task 2 demo posted (same rules)
- [ ] Task 5 demo posted (same rules)
- [ ] Substantive comments left on at least two cohort interns’ demos

### Final submission

- [ ] All notebooks re-run from fresh kernels; READMEs and GitHub files quality-checked
- [ ] Public `OIBSIP` link and demo links ready for the official form
- [ ] Submitted through the official Oasis Infobyte form by 15 November 2026
- [ ] Confirmed with the cohort whether there are earlier task-level dates (the letter says one month; confirm before relying on 15 November)

## Academic integrity

All code, analysis, and writing here is my work, produced with tutor guidance and tool assistance as permitted by Oasis Infobyte’s AI-use policy. I can explain every cell and every result in these notebooks. No scores, charts, screenshots, or findings in this repository are fabricated or marked complete before I have actually produced them.
