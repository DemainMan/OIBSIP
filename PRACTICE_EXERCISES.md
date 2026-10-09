# Practice Exercises

Extra problems I work through to build skill, separate from the three
internship tasks. Any synthetic data used here is **clearly labelled as
practice data** — it is never used as internship task data, and never mixed
into the real datasets.

---

## Exercise set 1 — Python and pandas basics (not started)

- [ ] **1.1** Load a small dictionary into a DataFrame and print `.shape`, `.dtypes`
- [ ] **1.2** Count nulls per column with a single pandas call
- [ ] **1.3** Filter rows by a condition and compute a group-by mean
- **TODO:** Write one sentence per exercise describing what I learned

## Exercise set 2 — Visualisation (not started)

- [ ] **2.1** Make a scatter plot with labelled axes, title and legend (matplotlib)
- [ ] **2.2** Make a box plot of a numeric column grouped by a category (seaborn)
- [ ] **2.3** Build a correlation heatmap and read it aloud to myself
- **TODO:** Write the observation I would add under each chart in a task notebook

## Exercise set 3 — Modelling hygiene (not started)

- [ ] **3.1** Reproduce the same train/test split twice using `random_state`
- [ ] **3.2** Build a `Pipeline` with `StandardScaler` + classifier, then confirm the scaler was fit on training data only
- [ ] **3.3** Print a classification report and explain every metric in it
- **TODO:** Note one mistake I made and how I spotted it

## Exercise set 4 — Visualisation practice: the Wine dataset (not started)

**Practice only.** This uses scikit-learn's built-in **Wine** dataset and is
completely separate from the Iris internship task. None of it is internship data
or an internship result.

- [ ] **4.1** Load the Wine dataset with `load_wine(as_frame=True)` and build a
  DataFrame with readable class names (map the numeric target to
  `wine.target_names`).
- [ ] **4.2** Make a pair plot (`seaborn.pairplot`) coloured by wine class using
  only the feature columns — keep the target column out of the plot.
- [ ] **4.3** Make a small grid of box plots (`seaborn.boxplot`), one panel per
  feature, grouped by wine class.
- [ ] **4.4** Save the figures into a clearly named practice folder (for example
  `practice_figures/`) so they are never confused with task outputs.
- **TODO (reflection, in my own words):** which Wine features look most
  discriminative, and how is reading these charts the same as or different from
  reading the Iris charts?

Do not mark this set complete until I have actually run it and written the
reflection myself.

## Synthetic-data rule

Synthetic rows created for practice live only in this file or in clearly
labelled practice notebooks. They must never be saved into
`DataScience-Task*/data/` or described as internship dataset content.
