Author: Zeyad Mohamed Arafat
Contact: zeyadarafat833@gmail.com

Linear Regression — Student Performance
=====================================

Overview
--------
This repository contains a Jupyter Notebook that implements a simple multivariate linear regression model (from scratch) to predict a "Performance Index" for students using the provided `Student_Performance.csv` dataset.

Files
-----
- linear-regression.ipynb — Notebook with the full workflow: data loading, preprocessing, model training (gradient descent), prediction, and a final scatter plot of true vs predicted values.
- Student_Performance.csv — Dataset used by the notebook.

Dependencies
------------
- Python 3.8+ recommended
- numpy
- pandas
- matplotlib

Install dependencies:

```powershell
pip install numpy pandas matplotlib
```

Notebook workflow (high level)
------------------------------
1. Load `Student_Performance.csv` with pandas and inspect the data.
2. Check for missing values and duplicates; drop duplicates.
3. Encode the `Extracurricular Activities` column to numeric (Yes=1, No=0) and remove the original column.
4. Split dataframe into features (X) and target (`Performance Index`).
5. Add a bias column to X and initialize `weights` to zeros.
6. Implement batch gradient descent (manual loop) to learn weights:
	- learning rate used in the notebook: 1e-8
	- iterations: 10,000
7. Compute predictions, report mean error, and plot true vs predicted values.

Notes
-------------------
- The notebook uses a very small learning rate and no feature scaling; consider normalizing features or using a larger learning rate with proper tuning.
- Add a train/test split for better evaluation.

How to run
----------
1. Open `linear-regression.ipynb` in Jupyter or VS Code and run the cells sequentially.
2. Ensure `Student_Performance.csv` is in the same folder as the notebook.

