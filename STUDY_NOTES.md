# Study Notes

My own notes on concepts learned during the Oasis Infobyte Data Science
internship. Everything here is written in my own words from things I have
actually run and understood. Nothing is marked as learned until I can explain
it without looking.

---

## Task 1 — Iris Flower Classification (not started)

- **TODO:** What a dataset "shape" is and why we check it
- **TODO:** Why we check dtypes and null values before modelling
- **TODO:** What a train/test split is, and what stratification does
- **TODO:** What data leakage is and how pipelines prevent it
- **TODO:** Difference between Logistic Regression, KNN and Decision Tree (in my own words)
- **TODO:** What the confusion matrix cells mean
- **TODO:** Precision vs recall vs F1 — when each matters
- **TODO:** Why feature scaling matters for some models and not others

### Visualisation concepts (study notes)

These are general explanations that help me read my own charts later — they are
not results from the Iris data.

- **Pair plot (scatter matrix):** plots every numeric feature against every other
  numeric feature in a grid. The diagonal usually shows each feature's own
  distribution (histogram or density); each off-diagonal panel is a scatter plot
  of one feature versus another. Colouring the points by the label (species)
  shows whether the classes form separate clumps or overlap.
- **Box plot:** summarises one numeric feature for each category. The box spans
  the middle 50% of the values (the interquartile range, Q1–Q3); the line inside
  is the median; the whiskers extend to the rest of the range (by the common
  1.5 × IQR rule); and dots beyond the whiskers are potential outliers.
  Comparing box heights shows which groups are more spread out or shifted.
- **Discriminative feature:** a feature is discriminative if its values differ
  enough between classes that it helps tell them apart. On a pair plot this looks
  like well-separated colour groups; on box plots it looks like boxes that sit at
  different levels with little overlap. A non-discriminative feature has heavily
  overlapping groups, so it carries little separating information.

**Reflection prompt (fill in myself after doing it):** _Which of these terms can
I now explain without looking, and which one is still fuzzy?_

## Task 2 — Unemployment Analysis (not started)

- **TODO:** Cleaning column names and whitespace — why it matters
- **TODO:** What happens when date parsing fails, and why I report those rows
- **TODO:** Correlation vs causation — the distinction in my own words
- **TODO:** What a correlation heatmap can and cannot tell me
- **TODO:** Why the pre/post-COVID cutoff must be defined explicitly

## Task 5 — Sales Prediction (not started)

- **TODO:** What a linear regression coefficient means
- **TODO:** MAE vs RMSE — how they differ and when RMSE punishes harder
- **TODO:** What R-squared does and does not tell me
- **TODO:** What a residual plot shows and what a good one looks like
- **TODO:** Why feature importance ≠ causation (my own example)

## General

- **TODO:** How to read my `.venv` setup and `pip install -r requirements.txt`
- **TODO:** What `random_state` does for reproducibility
- **TODO:** How to restart and re-run all cells in PyCharm/Jupyter
