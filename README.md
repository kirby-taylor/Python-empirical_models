# PROJECT 1 (audi_price_analysis.ipynb)
**Name**: 
Multiple Linear Regression for Real-World Pricing Models

**Problem**: 
Standard valuation models (eg KBB, NADA) do not account for how salvage titles affect vehicle prices.

**Approach**: 
This project attempts to reverse-engineer how local dealerships price vehicles with salvage titles by modeling listing data using multiple linear regression.

**Dataset**: 
Collected data for 102 local Audi A3 and A4 vehicles for sale online, with 18 features per entry (e.g., mileage, trim, year, condition).  
- See audi_dataset(5).xlsx for raw data and snippet-data_key.png for a variable reference guide.
- Note: due to limited salvage listings for A3s, A4s were included to strengthen the regression.

**Code Highlights:**  
- Uses pandas for data cleaning and imputation (e.g., fills missing mileage with median)
- Applies one-hot encoding to handle categorical variables
- Fits a linear regression model using Scikit-learn
- Calculates:
> R² score to evaluate model accuracy

> Coefficients to estimate price influence of each feature
- Accepts live vehicle input (via user prompt) and returns a real-time price prediction

**How it Works**
**1. Preprocessing**
- Boolean features (e.g., salvage, rims) are filled with 0
- Numeric values (e.g., milage, kbb_high) filled with median
- Categorical features (e.g., model, transmission) filled with mode and one-hot encoded
**2. Training**
- Dataset split 80/20 into training and test sets
- Model trained using LinearRegression() from Scikit-learn
**3. Evaluation**
- Compares model prediction vs. actual using R²
- Includes a baseline prediction using KBB High value
- Visuals show performance and feature impact
**4. Prediction**
- Accepts custom user input through prompts
- Aligns user input to model structure
- Outputs a price prediction with formatting

### Files Included
- `audi_price_analysis(5).ipynb` – Main analysis notebook (5th revision)
- `audi_dataset(5).xlsx` – Dataset used in the model  
- `snippet-data_key.png` – Reference guide to dataset variables (previous model)
- `snippet-graph-importance_of_features.png` – Feature importance graph (previous model)
- `snippet-graph-milage_vs_price.png` – Mileage vs. price graph (previous model)
