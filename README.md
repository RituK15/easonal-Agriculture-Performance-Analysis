Problem Statement

Farming in India doesn't follow one steady rhythm — it shifts across three seasons: Kharif, Rabi, and Zaid, each bringing its own rainfall, temperature, humidity, and soil conditions. Because of this, no two seasons produce the same results, but raw farm data alone doesn't explain how big these gaps are, what's causing them, or which farms are bucking the trend.

This project analyzes a dataset of 4,000 farm records spanning 8 Indian states and 8 crops to determine whether seasonal differences in yield, production, revenue, cost, and profit are statistically significant, identify which environmental and resource factors drive these differences, and pinpoint specific season–crop–state combinations that deviate from the general pattern.

Project Description

This project looks at how farming outcomes in India shift across the three cropping seasons — Kharif, Rabi, and Zaid — using a dataset of 4,000 farm records spanning 8 states and 8 crops.

Each record includes weather conditions, soil health, farming inputs (fertilizer, pesticide, irrigation, water usage), and financial results (production, revenue, cost, profit). Using Python (pandas, NumPy, Matplotlib, Seaborn, SciPy), the data was cleaned, missing values and outliers handled, and a few extra features like profit margin added to make comparisons easier.

The analysis covers:

Yield, output, and profit differences across seasons
Seasonal weather and environmental patterns
Which farm characteristics vary most by season
Crop and irrigation choices across seasons
Resource usage (water, fertilizer, pesticide) by season
Links between weather conditions and yield
An ANOVA test to confirm seasonal differences are statistically real
Standout exceptions — states or crops that break the usual pattern

The full analysis, from raw data to final insights, is documented in a Google Colab notebook — combining code, charts, and interpretation in one place.

Dataset
File: seasonal_agriculture_performance_dataset.csv
Records: 4,000 farms
Coverage: 8 states, 8 crops, 3 seasons (Kharif, Rabi, Zaid)
Key fields: environmental conditions (rainfall, temperature, humidity, soil pH/moisture), resource inputs (fertilizer, pesticide, irrigation method, water usage), and financial outcomes (yield, production, revenue, cost, profit)
Technology Used
Python — core language for the analysis
Pandas & NumPy — data loading, cleaning, and feature engineering
Matplotlib & Seaborn — visualizations (histograms, boxplots, bar charts, heatmaps, scatter plots, pie charts, violin plots)
SciPy (stats module) — ANOVA significance testing
Google Colab — notebook environment
Key Findings
Kharif season shows the highest average yield, revenue, and profit among the three seasons.
Zaid season shows the weakest performance, with the highest share of loss-making farms and the lowest water-use efficiency.
Rabi performs moderately, benefiting from more stable conditions than Zaid but without Kharif's rainfall advantage.
ANOVA testing confirms these seasonal differences are statistically significant (not random variation).
The environment–yield relationship differs by season — the same rainfall increase affects yield differently depending on the season's baseline conditions.
A few specific crop–state–irrigation combinations (e.g., Zaid with drip irrigation) remain profitable even in the otherwise weaker season.
End Users
Farmers deciding which crop and irrigation setup to use in a given season
Agricultural extension officers giving season-specific advice
State agriculture departments planning seasonal advisories and subsidies
Agri-businesses planning around seasonal production swings
Banks and crop insurance providers assessing seasonal risk
Students and researchers studying applied agricultural data analytics
How to Run
Open Seasonal_Agriculture_Performance_Analysis.ipynb in Google Colab.
Upload seasonal_agriculture_performance_dataset.csv when prompted (or mount Google Drive if the file is stored there).
Run all cells (Runtime → Run all).
Future Scope
Extend the analysis to multiple years of data to check whether seasonal patterns hold over time.
Incorporate real-time weather and market price feeds for live decision support.
Expand dataset coverage to more states, districts, and crop varieties.
Build a predictive model to estimate yield/profit before a season begins.
Create a simple dashboard for farmers and officers to access insights directly.
Bring in satellite/remote-sensing data for sharper environmental analysis.
Factor in climate change projections and policy shifts for longer-term relevance.
