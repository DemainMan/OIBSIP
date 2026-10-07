# Task 1 — Iris Flower Classification

**Intern:** Aphile Ashley · **Track:** Data Science · **Status:** Not started

## Objective

Classify iris flowers into their three species from sepal and petal
measurements, comparing at least two classifiers on a held-out test set.

## Dataset and source

- **Dataset:** Iris flower dataset
- **Source:** Loaded directly from `sklearn.datasets.load_iris()` — no external
  download required, no files needed in `data/`
- **Rows / features:** 150 rows, 4 numeric features (sepal length, sepal width,
  petal length, petal width), 3 classes (setosa, versicolor, virginica)

## Tools and environment

- Python 3, project `.venv`
- pandas, numpy, matplotlib, seaborn, scikit-learn
- Jupyter notebook: [`AphileAshley_Task1.ipynb`](AphileAshley_Task1.ipynb)

## How to run

1. Activate the project virtual environment (`source .venv/bin/activate`)
2. `pip install -r ../requirements.txt` (if not already installed)
3. Open `AphileAshley_Task1.ipynb`
4. Restart the kernel and run all cells top to bottom

## Methods

- **TODO:** data inspection (shape, dtypes, nulls, descriptive stats, class counts)
- **TODO:** pair plot / scatter matrix and box plots by species
- **TODO:** reproducible stratified ~80/20 train/test split
- **TODO:** models trained (e.g. Logistic Regression, KNN / Decision Tree) inside scaling pipelines
- **TODO:** evaluation metrics used (accuracy, confusion matrix, precision, recall, F1)

## Findings

> This section is filled in only after I have run the notebook and read its
> real outputs. Nothing here is pre-written.

- **TODO:** which measurements appear most discriminative, based on my charts
- **TODO:** per-model test results (real numbers from my run)
- **TODO:** which model I selected and why, based on actual test results

## Limitations

- **TODO:** dataset size and what it means for generalisation
- **TODO:** metrics/splits I would improve with more time
- **TODO:** anything I could not verify

## Submission tracking

- [ ] Notebook runs end to end from a fresh kernel
- [ ] Written interpretations completed by me
- [ ] Screenshots / outputs saved as required
- [ ] Demo video recorded (title card: full name, Data Science track, task title)
- [ ] LinkedIn post published with tag + `#oasisinfobyte`
