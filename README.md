# Retail Transactions Insights — Exploratory Data Analysis

This project explores a retail transactions dataset using Python, data manipulation, and visualization. It was developed as an Exploratory Data Analysis (EDA) assignment.

## Objectives

- Inspect the dataset shape and descriptive statistics.
- Parse transaction dates and derive year, month, month name, and day-of-week features.
- Check missing values and duplicate rows, and remove duplicate rows in the working DataFrame.
- Explore transaction counts, unique customers, popular products, and transaction distribution by city.
- Analyze spending by customer category, payment-method usage, and basket size by store type.
- Compare spending and item counts across discount and promotion groups.
- Explore revenue and transaction patterns by season.
- Visualize city transaction counts, payment-method distribution, monthly revenue, and revenue by season and customer category.

## Tech stack

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Repository contents

- `17_02_ASG1(1).ipynb` — original notebook, included without modifications.
- `requirements.txt` — Python package dependencies.
- `.gitignore` — ignores common local Python/Jupyter files.
- `data/README.md` — notes about the dataset.

## Dataset

The notebook expects a file named `Retail_Transactions_Dataset.csv`. The dataset itself is not included in this repository.

The original notebook currently reads the CSV from this local Windows path:

```python
pd.read_csv(r"Retail_Transactions_Dataset.csv")
```

To run the notebook on another machine, place the dataset somewhere accessible and update that path in the notebook yourself. The notebook has intentionally been left unchanged for this repository preparation.

Only publish the dataset if you have permission to redistribute it and it contains no sensitive information.

## Setup

Create and activate a virtual environment if desired, then install the dependencies:

```bash
python -m venv .venv
```

Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

macOS/Linux:

```bash
source .venv/bin/activate
```

Install packages:

```bash
pip install -r requirements.txt
```

Launch Jupyter:

```bash
jupyter notebook
```

Open `retail_transaction_insights.ipynb` and run the cells in order after making sure the dataset path points to your local CSV file.

## Scope and limitations

This repository documents an exploratory analysis notebook, not a deployed application. Findings depend on the supplied dataset and should not be interpreted as causal evidence. For example, differences between promotion groups alone do not prove that a promotion caused higher spending.

## Future improvements

- Make the dataset path configurable without machine-specific absolute paths.
- Add a data dictionary and document dataset provenance.
- Add more robust validation for missing or malformed values.
- Summarize the main findings and recommendations in a concise report.
#
