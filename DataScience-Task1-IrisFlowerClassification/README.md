# Task 1 — Iris Flower Classification

**Intern:** Aphile Ashley · **Track:** Data Science
**Status:** **In progress — setup/data inspection, visualizations, stratified split, chart observations recorded; two baseline classifiers trained on the training set; test evaluation complete (both 28/30 correct on held-out set; Logistic Regression more balanced across versicolor/virginica); model selection and conclusions recorded; fresh-kernel run verified**

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
- A species-coloured pair plot was generated from the real data using only the four measurement columns plus `species`.
- Four box plots (one per measurement) grouped by species were generated; the numeric `target` was excluded from the plotted frame.
- A reproducible stratified 80/20 train/test split was added using the four measurement features (`iris.data`) and the species target (`iris.target`) with `random_state=42` and `stratify=y`. The split was verified to give **120 training rows and 30 test rows**, with **40 of each species in training and 10 of each in the test set**.

**Visualizations, the train/test split, and the chart observations are recorded and verified.** The chart-observation section is now present in the notebook. Both baseline pipelines (Logistic Regression and K-Nearest Neighbors with StandardScaler) were fitted on `X_train, y_train`. Test evaluation and comparison are complete; model selection and conclusions are recorded. The notebook has been rerun end to end from a fresh kernel (verified). Remaining items: save relevant screenshots/output files if required, record the demo with the required title card, post/link on LinkedIn (tag Oasis Infobyte, include #oasisinfobyte), and address remaining submission items.

**Figure-path note:** the notebook saves PNGs to a relative `figures/` directory, so the location depends on the working directory used to launch it. The verified fresh-kernel run (launched from the repository root) wrote `figures/task1_pairplot.png` and `figures/task1_boxplots.png` at the repository root; copies from an earlier run (launched from this task folder) sit in `DataScience-Task1-IrisFlowerClassification/figures/` with the same filenames but different file contents. Both committed sets are left in place as-is.

## Tools and environment

- Python 3 in the project `.venv`
- pandas, numpy, matplotlib, seaborn, scikit-learn
- Jupyter notebook: [`AphileAshley_Task1.ipynb`](AphileAshley_Task1.ipynb)

## How to run

1. Activate the project virtual environment (`source .venv/bin/activate` on Linux/macOS; use the Windows activation command on Windows).
2. Install dependencies from the repository root with `pip install -r requirements.txt` if needed.
3. Open `AphileAshley_Task1.ipynb` in PyCharm and select the project `.venv` as its kernel.
4. Restart the kernel and run the notebook cells from top to bottom to reproduce the analysis.

## Methods and task checklist

- [x] Load the built-in Iris data and create readable species labels
- [x] Inspect shape, data types, null counts, descriptive statistics, and species counts
- [x] Pair plot/scatter matrix showing feature distributions by species
- [x] Box plots for each feature
- [x] Discuss which features appear most discriminative based on the plots
- [x] Reproducible approximately 80/20 train/test split using `train_test_split` and `stratify=y`
- [x] Train at least two classifiers; use a scaling pipeline for scale-sensitive models
- [x] Evaluate each model using accuracy, confusion matrix, precision, recall, and F1
- [x] Select and justify the best-performing model using actual held-out results
- [x] Rerun the notebook end to end from a fresh kernel (verified)
- [x] Final clean-and-commented polish pass on the notebook cells

## Findings

- **Discriminative features (charts):** Petal length and petal width separate the species most clearly, especially setosa; versicolor and virginica show some overlap.
- **Test results (held-out set, 30 samples):** Logistic Regression — accuracy 0.9333 (28/30). Confusion (true rows): setosa [10,0,0], versicolor [0,9,1], virginica [0,1,9] (P/R/F1 ~0.90 for versicolor/virginica). K-Nearest Neighbors — accuracy 0.9333 (28/30). Confusion: setosa [10,0,0], versicolor [0,10,0], virginica [0,2,8] (all versicolor found, two virginica misclassified as versicolor; versicolor precision ~0.83, virginica recall ~0.80). Both models achieve **28/30 correct**.
- **Model selection (on this split):** **Logistic Regression** is selected because it is more balanced across versicolor and virginica (precision/recall ~0.90 each), while KNN trades some precision for perfect versicolor recall. This choice is based on class-level metrics on this single split; it does not guarantee LR will always be better.

## Limitations

- Only 30 held-out flowers from one stratified split, so results may vary on other splits or datasets.
- Hyperparameters were not tuned, so the selection of Logistic Regression is specific to this split and does not guarantee future performance.
- The observed associations do not imply causation.

## Submission tracking

- [x] Rerun the full notebook from a fresh kernel (verified)
- [x] Remaining analysis completed (evaluation, comparison, model selection, and conclusions recorded above)
- [x] Add my chart observations, model comparison, and limitations
- [x] Save relevant screenshots/output files as required
- [ ] Record a functioning demo with the required 2-second title card
- [ ] Post/link the demo on LinkedIn, tag Oasis Infobyte, and include `#oasisinfobyte`
