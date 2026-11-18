# Residential Property Price Prediction
 
Multiple linear regression analysis of house sale prices in Ames, Iowa. Course final project, MS in Applied Data Science, University of Chicago.
 
**Research question:** How are property characteristics associated with sale prices, and how accurately can multiple linear regression predict prices for unseen properties?
 
## Team (Group 3)
 
- Michael Lin
- Sophie Jiang
- Yaxing Huang
## Data
 
- **Source:** Kaggle competition [House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview).
- **Original dataset:** the Ames Housing dataset, compiled by Dean De Cock from Ames City Assessor's Office records of residential sales from 2006 to 2010.
- **File used:** `train.csv` (1,460 sales with sale prices). Kaggle's `test.csv` has no sale prices, so it is not used.
- **Variables used:** `SalePrice` (response) and six predictors: `GrLivArea` (living area), `OverallQual` (overall quality), `HouseAge` (`YrSold − YearBuilt`), `TotalBsmtSF` (basement area), `GarageCars` (garage capacity), `Neighborhood`.
The data are not included in this repository. See *How to run* for download steps.
 
## Tools
 
| Purpose | Tool |
|---|---|
| Language | Python 3.10+ |
| Report and analysis | Jupyter Notebook |
| Data handling | pandas, NumPy |
| Model estimation and statistical tests | NumPy and SciPy (OLS implemented from the matrix formulas) |
| Train/test split and cross-validation | scikit-learn |
| Figures | Matplotlib |
| Version control | Git and GitHub |
 
## Approach
 
- **Model:** ordinary least squares on log sale price, with neighborhood as dummy variables and HC3 robust standard errors.
- **Variable selection:** candidate models compared with nested F-tests, AIC/BIC, and 5-fold cross-validation.
- **Diagnostics:** residual plots, Breusch–Pagan test, variance inflation factors, Cook's distance.
- **Evaluation:** 80/20 train/test split; RMSE, MAE, and R² in dollars.
- **Sensitivity analysis:** predicted price as living area and overall quality vary, other characteristics held fixed.
## Results
 
<!-- TODO: fill in from final_report.ipynb after running it on the real data -->
 
| | Training | Test |
|---|---|---|
| RMSE (USD) | TODO | TODO |
| MAE (USD) | TODO | TODO |
| R² | TODO | TODO |
 
## Repository contents
 
| Path | Contents |
|---|---|
| `final_report.ipynb` | Final report: full analysis, reproduces every result in the slides |
| `figures/` | Figures exported by the notebook |
| `slides/` | Final presentation |
| `data/` | Local only; place `train.csv` here (not tracked by Git) |
 
## How to run
 
1. Install dependencies: `pip install numpy pandas scipy scikit-learn matplotlib jupyter`
2. Download `train.csv` from the [Kaggle data page](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data) (free account required) and save it as `data/train.csv`.
3. Open `final_report.ipynb` and choose *Kernel → Restart & Run All*. A fixed random seed makes the results identical on every run.
 
## References
 
- Montoya, A., & DataCanary. (2016). *House Prices - Advanced Regression Techniques*. Kaggle. https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques
- De Cock, D. (2011). Ames, Iowa: Alternative to the Boston Housing Data as an End of Semester Regression Project. *Journal of Statistics Education*, 19(3).
 
