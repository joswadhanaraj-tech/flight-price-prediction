# Flight Price Prediction

This project explores flight fares and trains regression models to estimate ticket prices from flight details. The analysis and model evaluation are implemented in a Jupyter notebook, using the included Excel workbook as the dataset.

## Project files

- `Flight_Price_Prediction.ipynb.ipynb` — notebook containing data exploration, preprocessing, visualizations, model training, and evaluation.
- `Flight_Fare.xlsx` — flight fare dataset read by the notebook.

Keep the notebook and workbook in the same directory; the notebook loads the workbook using the relative path `Flight_Fare.xlsx`.

## Requirements

- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- openpyxl

## Setup

From the project directory, create and activate a virtual environment, then install the dependencies:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install pandas numpy matplotlib seaborn scikit-learn openpyxl notebook
```

Start Jupyter and open the project notebook:

```powershell
jupyter notebook
```

In Jupyter, open `Flight_Price_Prediction.ipynb.ipynb` and run the cells from top to bottom.

## Analysis workflow

The notebook:

1. Loads and inspects the fare data, including missing values, duplicates, column types, and distributions.
2. Cleans duplicate records and explores fare patterns with plots.
3. Extracts journey date, departure and arrival time, duration, and stop-count features.
4. One-hot encodes categorical variables and separates the features from the `Price` target.
5. Splits the data into training and test sets, then trains Linear Regression, Decision Tree, and Random Forest regressors.
6. Compares the models using MAE, RMSE, and R², and examines Random Forest feature importance and an example prediction.

The notebook is an analysis and evaluation workflow; it does not provide a deployed prediction service or save a trained model for later use.
