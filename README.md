# Insurance Cost Prediction

A notebook-based machine learning project that explores how demographic and lifestyle information relates to individual medical insurance charges. The project compares regression approaches and examines the effect of principal component analysis (PCA) on those models.

> **Project context:** Internship project. This repository presents an exploratory modeling workflow; its estimates are not insurance quotes or pricing decisions.

## What is in the repository

| File | Purpose |
| --- | --- |
| `ML Project - 3.ipynb` | Data exploration, preprocessing, model training, and comparison |
| `insurance.csv` | Input dataset used by the notebook |

The analysis considers attributes such as age, sex, number of children, and smoking status. The notebook compares a multiple regression model with a random forest model and investigates PCA variants. See the notebook output for the actual metrics and plots; this README does not assume an accuracy figure that may change when the notebook is rerun.

## Run the notebook

1. Clone the repository and move into its directory:

   ```bash
   git clone https://github.com/YashkumarJain/Insurance-Cost-Prediction.git
   cd Insurance-Cost-Prediction
   ```

2. Create a Python environment and install the notebook's core libraries:

   ```bash
   python -m venv .venv
   # macOS / Linux
   source .venv/bin/activate
   # Windows PowerShell: .venv\Scripts\Activate.ps1
   python -m pip install jupyter numpy pandas matplotlib scikit-learn
   ```

3. Launch Jupyter and open `ML Project - 3.ipynb`:

   ```bash
   jupyter notebook
   ```

4. Keep `insurance.csv` beside the notebook and run its cells in order. If a cell uses an absolute path from the original development machine, replace it with the relative filename `insurance.csv`.

## Workflow

1. Inspect the insurance dataset and explore the relationship between input attributes and charges.
2. Prepare the features for regression and split the data for evaluation.
3. Train and compare the regression and random forest approaches.
4. Examine how PCA changes the model comparison.

The notebook is the source of truth for the exact preprocessing, train/test split, hyperparameters, plots, and evaluation values.

## Scope and limitations

The dataset is a learning and experimentation resource. A model trained on it may not generalize to other populations, time periods, or insurance markets. The repository contains a notebook rather than a deployed prediction service. Avoid entering real personal information into a public notebook or committing it to this repository.

## Author

[Yashkumar Jain](https://github.com/YashkumarJain)
