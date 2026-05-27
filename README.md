# Perishable Inventory Demand Forecasting Engine

A demand forecasting pipeline for perishable SKUs (fruits, dairy) built to 
minimise total waste cost by combining stockout penalty and spoilage cost 
into a single optimisation objective.

## Tech Stack
Python, LightGBM, SHAP, Pandas

## Key Results
- MAPE of 8.3% vs 19.1% naïve baseline
- 21% reduction in simulated daily inventory loss
- Automated reorder-trigger system flagging SKUs crossing dynamic safety-stock thresholds
- Replenishment schedule designed for dark-store operating cadence

## Approach
- Engineered features for day-of-week seasonality, weather proxies, and promotional lift
- Applied SHAP explainability to surface top drivers of demand spikes
- Modelled spoilage cost as a function of over-ordering error
- Designed dynamic safety-stock thresholds per SKU category
