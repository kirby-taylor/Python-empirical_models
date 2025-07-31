# PROJECT 1 (audi_price_analysis.ipynb)
**Name**: 
Multiple Linear Regression for Real-World Pricing Models

**Problem**: 
Standard valuation models (eg KBB, NADA) do not account for how salvage titles affect vehicle prices.

**Approach**: 
This project attempts to reverse-engineer how local dealerships price vehicles with salvage titles by modeling listing data using multiple linear regression.

**Dataset**: 
Collected data for 102 local Audi A3 and A4 vehicles for sale online, with 18 features per entry (e.g., mileage, trim, year, condition).  
- See audi_dataset(3).xlsx for raw data and snippet-data_key.png for a variable reference guide.
- Note: due to limited salvage listings for A3s, A4s were included to strengthen the regression.

**Code Highlights:**  
- Uses pandas and numpy for data processing and modeling.
- Calculates R² score and regression coefficients.  
- Estimates the pricing value of individual features.  
- Outputs predicted listing price based on a vehicle’s attributes.
> Example graphs generated:
> snippet-graph-importance_of_features.png (feature weights)
> snippet-graph-milage_vs_price.png (relationship between mileage and price)

### Files Included
- `audi_price_analysis.ipynb` – Main analysis notebook  
- `audi_dataset(3).xlsx` – Dataset used in the model  
- `snippet-data_key.png` – Reference guide to dataset variables  
- `snippet-graph-importance_of_features.png` – Feature importance graph  
- `snippet-graph-milage_vs_price.png` – Mileage vs. price graph
