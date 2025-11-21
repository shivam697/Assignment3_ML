# MT25043 Assignment 3

Short description
- Jupyter notebook that performs EDA, preprocessing, feature engineering, and trains three classifiers (Decision Tree, Gradient Boosting, SVM).
- The main executable notebook is `MT25043_a3.ipynb`.

Files
- MT25043_a3.ipynb — main notebook with all code and instructions. See the classes and functions:
  - [`Dataset`](f:/ML Assignment/MT25043_a3/MT25043_a3.ipynb)
  - [`ModelTrainer`](f:/ML Assignment/MT25043_a3/MT25043_a3.ipynb)
  - [`get_decision_tree_classifier`](f:/ML Assignment/MT25043_a3/MT25043_a3.ipynb)
  - [`get_boosting_classifier`](f:/ML Assignment/MT25043_a3/MT25043_a3.ipynb)
  - [`get_svm_classifier`](f:/ML Assignment/MT25043_a3/MT25043_a3.ipynb)

Dataset
- Place the extracted `MLA3_DATA` folder next to the notebook (same directory).
  - Expected structure:
    - MLA3_DATA/TRAIN/train.csv
    - MLA3_DATA/TEST/student_test.csv
    - MLA3_DATA/TEST/hidden_test_sample.csv

How to run
1. Open `MT25043_a3.ipynb` in Jupyter / VS Code.
2. Do not change cells marked "DO NOT MODIFY THIS CELL".
3. Implement code only in sections labeled `# YOUR CODE HERE`.
4. Execute cells top-to-bottom.

What to modify
- Implement or tune preprocessing and feature engineering inside the `Dataset` class (`_load_and_preprocess`).
- Set hyperparameters in:
  - `get_decision_tree_classifier`
  - `get_boosting_classifier`
  - `get_svm_classifier`

Notes & grading
- Do not add/remove notebook cells or change function signatures — autograder depends on these.
- A small sample of the hidden test set is provided for preprocessing checks; final grading uses the full hidden set.
- Follow the notebook instructions for submission (rename notebook filename to your roll number as required).

Troubleshooting
- If preprocessing yields sparse matrices, the notebook converts them to dense arrays for compatibility.
- If sklearn version differences cause issues, check the code paths that import either `HistGradientBoostingClassifier` or fallback to `GradientBoostingClassifier`.

Contact
- Use the notebook comments/headers for further context.
