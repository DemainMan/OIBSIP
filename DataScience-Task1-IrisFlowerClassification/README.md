# Task 1 — Iris Flower Classification

**Intern:** Aphile Ashley · **Track:** Data Science  
**Status:** **In progress — setup/data inspection verified**

## Objective

Classify iris flowers into their three species from sepal and petal measurements, comparing at least two classifiers on a held-out test set.

## Dataset and source

- **Dataset:** Iris flower dataset
- **Source:** Loaded directly from `sklearn.datasets.load_iris()` — no external download is required.
- **Features:** Sepal length, sepal width, petal length, and petal width
- **Target:** Three species — setosa, versicolor, and virginica

## Progress verified so far

- The built-in Iris dataset was loaded and readable species names were added to the DataFrame.
- The inspected DataFrame has **150 rows and 6 columns**: four measurements, numeric `target`, and categorical `species`.
- The four measurements have `float64` dtype; `target` has `int64` dtype; `species` is categorical.
- Null counts are zero for every column.
- There are 50 records for each species.
- The notebook kernel was verified to use the project `.venv`.

**This verifies only the setup and initial data-inspection stage.** The visualizations, feature discussion, train/test split, models, evaluation, and conclusions have not yet been completed.

## Tools and environment

- Python 3 in the project `.venv`
- pandas, numpy, matplotlib, seaborn, scikit-learn
- Jupyter notebook: [`AphileAshley_Task1.ipynb`](AphileAshley_Task1.ipynb)

## How to run

1. Activate the project virtual environment (`source .venv/bin/activate` on Linux/macOS; use the Windows activation command on Windows).
2. Install dependencies from the repository root with `pip install -r requirements.txt` if needed.
3. Open `AphileAshley_Task1.ipynb` in PyCharm and select the project `.venv` as its kernel.
4. Restart the kernel and run the notebook cells from top to bottom as the task is developed.

## Methods and task checklist

- [x] Load the built-in Iris data and create readable species labels
- [x] Inspect shape, data types, null counts, descriptive statistics, and species counts
- [ ] Pair plot/scatter matrix showing feature distributions by species
- [ ] Box plots for each feature
- [ ] Discuss which features appear most discriminative based on the plots
- [ ] Reproducible approximately 80/20 train/test split using `train_test_split` and `stratify=y`
- [ ] Train at least two classifiers; use a scaling pipeline for scale-sensitive models
- [ ] Evaluate each model using accuracy, confusion matrix, precision, recall, and F1
- [ ] Select and justify the best-performing model using actual held-out results
- [ ] Complete a clean, commented notebook and rerun it from a fresh kernel

## Findings

> Complete this section only after running the remaining analysis. Use actual outputs and write interpretations I can explain.

- **TODO:** Which measurements appear most discriminative, based on my charts?
- **TODO:** What are the actual test results for each model?
- **TODO:** Which model do I select, and why?

## Limitations

- **TODO:** Discuss the dataset size and what it means for generalisation.
- **TODO:** Note limitations of the split/metrics and any uncertainty.
- **TODO:** State what I would improve with more time.

## Submission tracking

- [ ] Complete remaining analysis and rerun the full notebook from a fresh kernel
- [ ] Add my chart observations, model comparison, and limitations
- [ ] Save relevant screenshots/output files as required
- [ ] Record a functioning demo with the required 2-second title card
- [ ] Post/link the demo on LinkedIn, tag Oasis Infobyte, and include `#oasisinfobyte`
