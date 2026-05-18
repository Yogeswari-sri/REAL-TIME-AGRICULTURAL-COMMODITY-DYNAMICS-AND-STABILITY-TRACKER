# REAL-TIME-AGRICULTURAL-COMMODITY-DYNAMICS-AND-STABILITY-TRACKER 21-April-2026
This project demonstrates that agricultural market data, when structured into a dashboard, is not just a record of prices but a decision-support system. It empowers farmers to manage risk, traders to hedge against volatility, and policymakers to design targeted interventions. 



📌 Objectives
Monitor commodity prices (Min, Max, Modal) across districts and markets.

Classify commodities into Stable vs Volatile using the Price Stability Index.

Benchmark commodities (Wheat, Rice, Potato, etc.) across districts and grades.

Compare APMCs to highlight differences in price ranges and stability.

Assess grade and variety impact on stability and volatility.

Provide actionable insights for farmers, traders, and policymakers.
Objectives
Track Min, Max, Modal prices across districts and commodities.

Classify commodities into Stable vs Volatile using the Price Stability Index.

Benchmark commodities across districts, grades, and varieties.

Compare APMCs to identify regional differences in price ranges and volatility.

Provide actionable insights for farmers, traders, and policymakers to reduce risk.

🧹 Data Cleaning (Power Query / Excel)
Remove duplicates → Commodity names, districts, dates.

Handle missing values → Replace null prices with averages or flag them.

Standardize formats → Dates (YYYY-MM-DD), commodity names (trim spaces, proper case).

Outlier detection → Filter extreme price spikes using IQR or Z‑score.

Categorization → Assign grades (Local, FAQ, A, B, C) consistently.

Merge sources → Combine district‑level and commodity‑level tables with proper keys.

Data Modelling (Power BI / Excel Data Model)
Fact Table → Commodity Transactions (Date, District, Commodity, Price, Arrival Volume).

Dimension Tables →

Commodity Dimension (Name, Grade, Volatility Index).

District Dimension (Region, State, Country).

Date Dimension (Day, Month, Quarter, Year).

Relationships →

Fact ↔ Commodity (Many‑to‑One).

Fact ↔ District (Many‑to‑One).

Fact ↔ Date (Many‑to‑One).

Calculated Columns →

VolatilityFlag = IF([VolatilityIndex] > 1, "Volatile", "Stable")


✅ Outcome:  
This workflow ensures clean, consistent data, a robust star schema model, and DAX measures that capture volatility, stability, spreads, and benchmarks for actionable insights in real‑time dashboards.

📊 Visuals
Bar Chart – Price Range by Commodity

Pie Chart – Stability vs Volatility Distribution

clustered bar chart – District vs Price Stability Index

Line Chart – Modal Price Trends by Commodity

Clustered Column Chart – Grade vs Stability Category

Matrix stable - stability Rank Analysis

✅ Key Insights
43% of commodities show volatility, driven by perishability, seasonal cycles, and uneven supply chains.

Stable commodities (Wheat, Gram, Jaggery) provide predictable benchmarks, while volatile ones (Rice, Potato, Garlic, Tomato) remain unstable.

District disparities highlight urban markets with extreme fluctuations versus rural APMCs with relative stability.

Graded varieties (FAQ, standardized grades) reduce volatility compared to local varieties.

Real‑time monitoring enables early detection of instability and supports data‑driven interventions.

🧩 Analytics Framework

Descriptive Analysis (What happened?)
Rice, Potato, and BOP showed wide price spreads and volatility.

Wheat and Gram remained stable with consistent pricing.

Urban markets (Delhi, Kamrup) recorded extreme volatility, while rural APMCs showed stability.

Diagnostic Analysis (Why did it happen?)
Volatility driven by perishability, seasonal demand, and regional imbalances.

Stability linked to standardized FAQ grades and less perishable commodities.

Local varieties showed higher fluctuations compared to standardized grades.

Predictive Analysis (What is likely to happen?)
Volatile commodities (Rice, Potato, BOP) will continue instability unless supply chain improvements occur.

Stable commodities (Wheat, Gram) will remain benchmarks.

Seasonal cycles will reinforce stability in grains but increase volatility in perishables.

Prescriptive Analysis (What should we do?)
Optimize supply chains with cold storage and logistics.

Introduce price stabilization mechanisms (MSP, buffer stocks).

Diversify into stable commodities to balance volatility.

Promote standardized grades to reduce fluctuations.

Implement regional subsidies and trade agreements for high‑volatility districts.

DATA MODELLING OUTPUT



<img width="751" height="583" alt="mrkmodelling" src="https://github.com/user-attachments/assets/b1c0bc69-968b-4636-81b8-97c684a3104b" />


📑 Final Conclusion
The dashboard reveals a clear divide between stable commodities (Wheat, Gram, Jaggery) and volatile commodities (Rice, Potato, BOP). Stability is tied to standardized grades and non‑perishable items, while volatility stems from perishability, seasonal cycles, and regional demand.

By combining Descriptive, Diagnostic, Predictive, and Prescriptive analytics, the project transforms raw market data into actionable intelligence. It empowers farmers to manage risk, traders to hedge against volatility, and policymakers to design targeted interventions. Ultimately, this documentation provides a roadmap for stabilizing markets, improving profitability, and enhancing transparency in the agricultural economy.

OUTPUT OF DASHBOARD
🌾 Agricultural Commodity Market Dashboard
<img width="1526" height="735" alt="mmmm" src="https://github.com/user-attachments/assets/50efdfa5-ab73-4d63-8096-74e56299b14d" />

📑 Conclusion
The Agricultural Commodity Dynamics and Stability Tracker demonstrates that markets are highly dynamic, with volatility concentrated in perishable and regionally imbalanced commodities. By combining descriptive, diagnostic, predictive, and prescriptive analytics, the dashboard transforms raw data into actionable intelligence:

Farmers gain clarity on crop choices.

Traders can hedge against volatility.

Policymakers can design targeted interventions such as storage investment, cooperative marketing, and trade agreements.




