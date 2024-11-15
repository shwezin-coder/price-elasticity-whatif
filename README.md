Here's a README file draft for your GitHub repository:

---

# Price Elasticity Analysis with Power BI

This repository contains an analysis of **price efficiency** and a **what-if analysis** using Power BI, based on the AdventureWorks dataset. The main goal of this project is to explore price elasticity and its potential impact on product pricing strategy to maximize profitability.

## Overview

Price elasticity measures how demand changes in response to price adjustments:
- **|Price Elasticity| > 1 (Elastic)**: Indicates that a change in price significantly affects demand.
- **|Price Elasticity| < 1 (Inelastic)**: Suggests that a change in price has little impact on demand.
- **|Price Elasticity| = 1 (Unit Elastic)**: Implies that a 1% change in price results in a proportional 1% change in demand.

This analysis uses the midpoint formula for calculating percentage changes to ensure balanced interpretation:
- **Quantity Change (%)**:
 Quantity Changes (%) = (Current Qty - Previous Qty)/((Current Qty + Previous Qty)/2)
- **Price Change (%)**:
Price Changes (%) = (Current Price - Previous Price)/((Current Price + Previous Price)/2)

## Project Components

### 1. **Data Preparation**
   - Created a summarized price history table using DAX in Power BI.
   - Calculated **previous quantity** and **previous price** using time intelligence functions.

### 2. **Price Elasticity Calculation**
   - Implemented the following formula for Price Elasticity of Demand (PED):
PED = Quantity Changes (%)/ Price Changes(%)
  
### 3. **What-If Analysis**
   - Calculated the **adjusted quantity** to project potential outcomes based on changes in product prices:
   Adjusted Quantity = Old Quantity * (1 + (PED * Price Change))
    
   - Used the average price elasticity for this calculation due to minimal variance between average and median and low standard deviation.

## Findings
Most product categories in the dataset have higher average costs than selling prices, indicating a potential issue with the pricing strategy. The analysis helps identify which products may need price adjustments to improve profitability without significantly affecting sales volume.

## How to Use This Repository
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/price-elasticity-analysis.git
   ```
2. **Open the Power BI file** to explore the data model, DAX calculations, and visualizations.

## References
- [Khan Academy: Price Elasticity](https://www.khanacademy.org/economics-finance-domain/microeconomics/elasticity-tutorial/price-elasticity-tutorial/a/price-elasticity-of-demand-and-price-elasticity-of-supply-cnx)


## Contact
For any questions or feedback, please contact Daniel Hardin at hninshwezinhlaing05062001@gmail.com.

