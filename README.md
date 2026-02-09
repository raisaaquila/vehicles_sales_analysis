# Market Analysis and Inventory Strategy for Car Dealerships

This project provides a comprehensive framework for car dealerships to optimize their procurement and pricing strategies. By analyzing vehicle sales transactions from January 2014 to July 2015, the project identifies key drivers that cause a vehicle's actual selling price to deviate from the Manheim Market Report (MMR).

## Data Gaps & Context 
- Timeframe: Data covers transactions from 1 January 2014 to July 21, 2015.
  
- Missing Data: The dataset lacks transactions for August through November 2014.
  
- Baseline: 2015 is treated as "now" for vehicle age comparisons.

## Key Research Categories
**- Performance & Valuation (MMR vs. Actual):** Analyzing price variance, brand performance, and regional impacts.

**- Vehicle Attributes & Value Drivers:** Quantifying the impact of mileage, condition grades, and aesthetic choices.

## Strategic Project Findings
The analysis reveals several critical insights into how physical attributes and geography influence vehicle valuation:

**- The "Golden Unit" Profile:** The most profitable vehicle profile for a dealership is a 0–3 year old Suzuki, Acura, or Subaru with under 90,000 Km of mileage and a condition grade of 4.0 or higher. For maximum enthusiast demand, the ideal aesthetic is a Lime exterior paired with a Yellow interior.

**- Regional Price Arbitrage:** There is a theoretical 6–10% profit margin available simply by moving inventory from underperforming regions like Massachusetts to high-demand regions like Washington.

**- Discontinued Brand Risks:** Brands such as Saturn, Mercury, and Pontiac are severely underperforming due to a lack of official service channels. Dealers are advised to avoid these unless they can be acquired at least 15% below MMR.

**- Physical Value Drivers:** Mileage is the single most important factor, with cars exceeding 90,000 Km typically losing 2–5% of their market value.

Based on the data, dealers should adopt the following "Big Three" priorities when acquiring new inventory:
**- Strict Odometer Limit:** Prioritize units with under 90,000 Km to avoid the value "cliff".

**- Brand Stability:** Focus on Acura, Suzuki, or Subaru to ensure reliable demand.

**- Condition Threshold: **Only acquire units with a 4.0 grade or higher to avoid the 17% price penalty associated with lower-grade vehicles.

## Feature Importance Analysis
A Random Forest Regressor was utilized specifically for Feature Importance Analysis to determine which variables most significantly "move the needle" on a car's final price ratio.

The model identifies the following as the most critical predictors of price stability:
- Odometer (Mileage): The single most deciding price driver.
- Make: Brand manufacturer stability (e.g., Suzuki vs. Jaguar).
- Age: Younger cars (0-3 years) show the lowest variance from MMR.
- State: Geographical location provides significant profit authority.
- Condition Grade: Physical quality relative to the 4.0 benchmark.
