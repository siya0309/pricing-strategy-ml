
# Pricing Strategy Optimization System

## Project Overview

This project builds a machine learning system to recommend optimal product prices using historical retail data.

## Objectives

* Predict demand based on price
* Analyze price elasticity
* Recommend optimal pricing
* Maximize revenue

## Models Used

* Linear Regression
* Random Forest
* Gradient Boosting

## Features

* Feature engineering (log_price, price ratios, etc.)
* Cross-validation
* Demand vs Price visualization
* Revenue optimization
* Feature importance analysis

## Results

| Model             | CV RMSE | Test RMSE | R² Score |
| ----------------- | ------: | --------: | -------: |
| Linear Regression |  14.779 |    16.544 |   -0.010 |
| Random Forest     |  13.514 |    14.131 |    0.263 |
| Gradient Boosting |  14.030 |    13.649 |    0.313 |

 **Best Model:** Gradient Boosting



## Key Insights

* **Gradient Boosting** achieved the lowest test RMSE → best predictive performance
* **Linear Regression underperformed** → indicates non-linear relationship between price and demand
* **Tree-based models (RF & GB)** captured demand patterns more effectively
* Positive R² (~0.31) shows the model explains a meaningful portion of demand variation



##  Interpretation

* Demand is **not purely linear with price**
* Customer behavior is influenced by multiple factors (discounts, category, etc.)
* Machine learning models significantly improve pricing decisions over simple regression


## Business Takeaway

Using Gradient Boosting:

* Predict demand more accurately
* Identify optimal price points
* Improve revenue through data-driven price
* 
## Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

## Sample Outputs
<img width="1062" height="410" alt="image" src="https://github.com/user-attachments/assets/ced59866-173f-4302-a2c1-a00b2f454362" />
<img width="1157" height="426" alt="image" src="https://github.com/user-attachments/assets/e68448f6-e6a6-4659-9a09-47fd91ad52a6" />
<img width="755" height="551" alt="image" src="https://github.com/user-attachments/assets/2b3b6312-bd96-473c-977a-e01b1cba8f43" />
<img width="725" height="551" alt="image" src="https://github.com/user-attachments/assets/33ed4c40-6a4d-4924-9bf5-4d996179cdcf" />
<img width="711" height="541" alt="image" src="https://github.com/user-attachments/assets/f1df20f5-35ba-429e-bc28-01627c54796f" />



```bash
pip install -r requirements.txt
python src/pricing_model.py
```
