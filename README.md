<h1> Optimizing Inventory Value for Consumable Materials in a Leading Company with ANN </h1>

<h2>Description</h2>

<p align="justify"> To enhance time efficiency and ensure timely procurement, The Oil Company utilizes automated MRP through the SAP system. However, in recent years, The Oil Company has been conducting MRP planning manually. This shift is because minimum and maximum stock parameters in the SAP system have not been reviewed for several years, causing them unrepresentative of current demand.  Using outdated parameters can lead to inventory surplus, shortages, and elevated inventory values.  This project aims to review outdated inventory parameters and analyze the result of forecasting using a comparitive new method, specifically Artificial Neural Network, to identify potential cost savings.</p>


<h2>Tools Used</h2>

- <b>Ms Excel</b> 
- <b>Matlab (Neural Network Toolbox)</b


<h2>Methodology and Workflow</h2>
<p align="justify"> The parameter review analyzed a dataset of 645 entries categorized into 10 commodities: Absorbent, Cleaner Corrosion, Gasket Sheet, Grating, Lifting Material, Pipe Structure, Workshop Consumable, Turbine Cleaner, Various Bearings, and Valve Ball. Key attributes included material description, MAP (Moving Average Price), lead time (with and without contract), plant, unit, MRP type, LHG, existing ROP, safety stock, maximum inventory level, and historical demand (2020–2024). Two lead time scenarios were considered: with and without contracts, where the latter applies if The Oil Company lacks a vendor contract. New min-max parameters were calculated based on historical demand, and inventory value was derived by multiplying these parameters by MAP.  The Process of reviewing MRP parameter, forecasting material demand using ANN, and cost analysis can be seen below</p>

<p align="center">
<br/>
<img src="" height="50%" width="50%">
<br />

<p align="justify"> The MATLAB Neural Network Toolbox with backpropagation training was used for forecasting to streamline data processing. This method is chosen for its suitability with time series data.  Forecast result will then be used to calculate inventory value</p>


<h2>Results</h2>

