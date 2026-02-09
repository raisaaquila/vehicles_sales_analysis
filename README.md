# Market Analysis and Inventory Strategy for Car Dealerships

This project provides a comprehensive framework for car dealerships to optimize their procurement and pricing strategies. By analyzing vehicle sales transactions from January 2014 to July 2015, the project identifies key drivers that cause a vehicle's actual selling price to deviate from the Manheim Market Report (MMR).

## Data Gaps & Context 
- Timeframe: Data covers transactions from 1 January 2014 to July 21, 2015.
  
- Missing Data: The dataset lacks transactions for August through November 2014.
  
- Baseline: 2015 is treated as "now" for vehicle age comparisons.

## Key Research Categories
**- Performance & Valuation (MMR vs. Actual):** Analyzing price variance, brand performance, and regional impacts.
<img width="1479" height="4347" alt="a2532bc2-e3ed-4f0b-97c2-495ee8327d2d" src="https://github.com/user-attachments/assets/c791a026-de36-4015-8ef7-b6f3e9e7a6a9" />

**- Vehicle Attributes & Value Drivers:** Quantifying the impact of mileage, condition grades, and aesthetic choices.
<img width="1389" height="3845" alt="05e545e0-943a-4773-9f8a-6d0b952258bf" src="https://github.com/user-attachments/assets/4fcb782e-5d48-48ee-8ba6-2adbc95ca742" />

## Strategic Project Findings
The analysis reveals several critical insights into how physical attributes and geography influence vehicle valuation:

**- The "Golden Unit" Profile:** The most profitable vehicle profile for a dealership is a 0–3 year old Suzuki, Acura, or Subaru with under 90,000 Km of mileage and a condition grade of 4.0 or higher. For maximum enthusiast demand, the ideal aesthetic is a Lime exterior paired with a Yellow interior.

**- Regional Price Arbitrage:** There is a theoretical 6–10% profit margin available simply by moving inventory from underperforming regions like Massachusetts to high-demand regions like Washington.

**- Discontinued Brand Risks:** Brands such as Saturn, Mercury, and Pontiac are severely underperforming due to a lack of official service channels. Dealers are advised to avoid these unless they can be acquired at least 15% below MMR.

**- Physical Value Drivers:** Mileage is the single most important factor, with cars exceeding 90,000 Km typically losing 2–5% of their market value.

Based on the data, dealers should adopt the following "Big Three" priorities when acquiring new inventory:
**- Strict Odometer Limit:** Prioritize units with under 90,000 Km to avoid the value "cliff".

**- Brand Stability:** Focus on Acura, Suzuki, or Subaru to ensure reliable demand.

**- Condition Threshold:** Only acquire units with a 4.0 grade or higher to avoid the 17% price penalty associated with lower-grade vehicles.

## Feature Importance Analysis
A Random Forest Regressor was utilized specifically for Feature Importance Analysis to determine which variables most significantly "move the needle" on a car's final price ratio.

<img width="989" height="590" alt="3312c066-d210-4d53-8351-3707da37a56a" src="https://github.com/user-attachments/assets/c6b59930-680c-4ced-99bc-6cb0dcc14020" />

The model identifies the following as the most critical predictors of price stability:
- Odometer (Mileage): The single most deciding price driver.
- State: Geographical location provides significant profit authority.
- Make: Brand manufacturer stability (e.g., Suzuki vs. Jaguar).
- Color: Acts as a primary driver for market liquidity and rarity premiums.
- Interior: Acts as a proxy for vehicle grade and luxury tier.
