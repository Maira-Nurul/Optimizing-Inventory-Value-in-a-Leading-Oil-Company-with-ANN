<h1> Optimizing Inventory Value for Consumable Materials in a Leading Company with ANN </h1>

<h2>Description</h2>

<p align="justify"> To enhance time efficiency and ensure timely procurement, The Oil Company utilizes automated MRP through the SAP system. However, in recent years, The Oil Company has been conducting MRP planning manually. This shift is because minimum and maximum stock parameters in the SAP system have not been reviewed for several years, causing them unrepresentative of current demand.  Using outdated parameters can lead to inventory surplus, shortages, and elevated inventory values.  This project aims to review outdated inventory parameters and analyze the result of forecasting using a comparitive new method, specifically Artificial Neural Network, to identify potential cost savings.</p>


<h2>Tools Used</h2>

- <b>Ms Excel</b> 
- <b>Matlab (Neural Network Toolbox)</b>


<h2>Methodology and Workflow</h2>
<p align="justify"> The parameter review analyzed a dataset of 645 entries categorized into 10 commodities: Absorbent, Cleaner Corrosion, Gasket Sheet, Grating, Lifting Material, Pipe Structure, Workshop Consumable, Turbine Cleaner, Various Bearings, and Valve Ball. Key attributes included material description, MAP (Moving Average Price), lead time (with and without contract), plant, unit, MRP type, LHG, existing ROP, safety stock, maximum inventory level, and historical demand (2020–2024). Two lead time scenarios were considered: with and without contracts, where the latter applies if The Oil Company lacks a vendor contract. New min-max parameters were calculated based on historical demand, and inventory value was derived by multiplying these parameters by MAP.  The Process of reviewing MRP parameter, forecasting material demand using ANN, and cost analysis can be seen below</p>

<p align="center">
<br/>
<img src="https://github.com/Maira-Nurul/Optimizing-Inventory-Value-in-a-Leading-Oil-Company-with-ANN/blob/main/Docs%203/Screenshot%202025-01-08%20175511.png" height="50%" width="50%">
<br />

<p align="justify"> The MATLAB Neural Network Toolbox with backpropagation training was used for forecasting to streamline data processing. This method is chosen for its suitability with time series data.  Forecast result will then be used to calculate inventory value.</p>


<h2>Results</h2>
Based on the analysis, the following result has been found

<p align="center">
<br/>
<img src="https://github.com/Maira-Nurul/Optimizing-Inventory-Value-in-a-Leading-Oil-Company-with-ANN/blob/main/Docs%203/Screenshot%202025-01-08%20175558.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


- <p align="justify">Inventory values for Gasket Sheet, Valve Ball, and Various Bearing increased, with the highest rise seen in Valve Ball due to higher demand from unit replacements and maintenance activities. Intermittent demand for Valve Ball further raised its min-max parameters, despite not being consistently needed every year. Increased demand over the last 4 years caused higher stock parameters for Gasket Sheet and Various Bearing to maintain service levels. Seven other commodities saw a decrease in inventory levels due to reduced demand, which led to parameter adjustments to avoid surplus and lower inventory. Analysis also revealed that inventory levels would be lower with contracts, as these contracts shorten lead time. The review resulted in a negative savings of $2,591,035.64 (58% increase) when contracts were in place, and a larger increase of $4,093,582.86 (91%) without contracts.</p>
- <p align="justify">Forecasted demand using the ANN method was applied to calculate new stock parameters for Valve Ball. The analysis showed that inventory value increased from $1,263,201.96 (existing conditions) to $5,576,593.78 with average historical demand under contract (LTC), and $2,165,509.72 with forecasted demand under LTC. Although the inventory value increased, the rise was less significant compared to the existing method, as ANN better adjusted stock parameters for intermittent and fluctuating demand. <b>Overall, inventory value decreased by $820,048.42 (18%) with forecasted demand under contract and increased by 35% without contracts. It is recommended that the company secure procurement contracts for all 10 commodities.<b></p>
