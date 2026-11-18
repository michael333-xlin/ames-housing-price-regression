# Residential Property Price Prediction
 
Multiple linear regression analysis of house sale prices in Ames, Iowa. Course final project, MS in Applied Data Science, University of Chicago (Group 3: Michael Lin, Sophie Jiang, Yaxing Huang).
 
**Research question:** How are property characteristics associated with sale prices, and how accurately can multiple linear regression predict prices for unseen properties?
 
## Approach
 
- **Data:** 1,460 sales from the Ames housing dataset; six predictors (living area, overall quality, house age, basement area, garage capacity, neighborhood).
- **Model:** OLS on log sale price, with HC3 robust standard errors.
- **Evaluation:** 80/20 train/test split; RMSE, MAE, and R² in dollars.
## Results
 
<!-- TODO: fill in from final_report.ipynb after running it on the real data -->
 
| | Training | Test |
|---|---|---|
| RMSE (USD) | TODO | TODO |
| MAE (USD) | TODO | TODO |
| R² | TODO | TODO |
 
## How to run
 
1. Install dependencies: `pip install numpy pandas scipy scikit-learn matplotlib jupyter`
2. Download `train.csv` from [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data) and save it as `data/train.csv`.
3. Open `final_report.ipynb` and choose *Kernel → Restart & Run All*.
## Notes
 
Generative AI (Claude, Anthropic) was used to draft code; the team reviewed and verified all code and results.
<!-- TODO: edit to describe your actual AI use -->
 
Data: De Cock, D. (2011). Ames, Iowa: Alternative to the Boston Housing Data. *Journal of Statistics Education*, 19(3).
 
