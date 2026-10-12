# Study Notes

My own notes on concepts learned during the Oasis Infobyte Data Science
internship. Everything here is written in my own words from things I have
actually run and understood. Nothing is marked as learned until I can explain
it without looking.

---

## Task 1 — Iris Flower Classification (in progress)

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

### Stratification and data leakage (added after running the split)

- **Stratification:** when I split the data I passed `stratify=y` to
  `train_test_split`. This tells it to keep the same proportion of each class
  in both the training part and the test part. Because the Iris data has 50
  rows of each species, a stratified 80/20 split puts **40 of each species in
  training and 10 of each in the test set**. Without it, a plain random split
  could accidentally leave one part with very few rows of a species, which
  would make the results harder to trust.
- **Data leakage:** leakage is when information that should be hidden from the
  model sneaks into training, so the model looks better than it really is. The
  classic example is fitting something that learns from data (such as a scaler)
  or tuning choices on the whole dataset, including the test rows, before
  splitting. The fix is to split first, fit anything that learns from data on
  the training part only, and leave the test set untouched until the single
  final evaluation.

**Reflection prompt (fill in myself after doing it):** _Can I explain, in my own
words, why the test set must stay untouched until the end, and what leakage
would do to my results?_

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
