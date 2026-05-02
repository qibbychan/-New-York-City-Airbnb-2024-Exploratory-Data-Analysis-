**🗽 New York City Airbnb 2024 — Exploratory Data Analysis**

What does it actually cost to stay in New York City and does where you sleep really matter?

This project digs into 20,000+ real Airbnb listings across New York City to uncover pricing patterns, neighbourhood dynamics, and the types of stays that dominate the market. Using Python for end-to-end analysis, the goal wasn't just to clean data — it was to ask real questions and let the data answer them.

🧭 New York City is one of the most visited cities in the world. With thousands of Airbnb listings spread across five boroughs, the data tells a story about how people travel, where they stay, and how much they're willing to pay.
Some questions I wanted to answer going in:

- 🏘️ Which neighbourhoods command the highest prices — and is the premium worth it?
- 🛏️ What type of room do most travellers actually book?
- 📉 Are cheap listings actually available, or are they always booked out?
- 🧹 How messy is real-world data, and what does cleaning it actually involve?


🔍 Key Findings

🛏️ Room Types — The Market Is More Divided Than You'd Think
Entire home/apartment listings dominate the platform, but private rooms are far more common than most people assume — making NYC Airbnb surprisingly accessible for budget travellers who don't need a whole apartment to themselves. Shared rooms, however, are nearly extinct on the platform.

🗺️ Neighbourhood Matters — A Lot
Manhattan listings sit at a significant price premium over outer boroughs like the Bronx and Staten Island. But Brooklyn tells an interesting middle story — high demand, competitive pricing, and the widest variety of room types of any borough.

📊 Outliers Are Everywhere
Some listings were priced at $0. Others at $10,000+ per night. Real-world data is messy — and filtering outliers responsibly (without just deleting everything inconvenient) was one of the most important analytical decisions in this project.

📅 Availability ≠ Popularity
High availability doesn't mean a listing is good — it often means it's new or underperforming. The most-reviewed listings tend to have tighter availability windows, suggesting demand drives bookings more than price alone.

⚙️ What Was Done
StageDetailsData LoadingImported 20,000+ listings from the NYC Airbnb 2024 datasetData Exploration.info(), .describe(), null value mapping, data typesData CleaningHandled missing values, removed duplicates, fixed data typesUnivariate AnalysisPrice distribution, room type counts, availability histogramsOutlier HandlingIQR-based filtering for price anomaliesBivariate AnalysisPrice vs neighbourhood, room type vs reviews, host listings countFeature EngineeringCreated new columns to extract deeper patternsAdvanced AnalysisCorrelation heatmap, groupby aggregations, pairplots

💡 My Own Questions (Beyond the Tutorial)
While following the project structure, I paused to ask questions the tutorial didn't explicitly answer:

- "If entire apartments dominate, who is the private room market actually for?"
- "Does a higher number of reviews always mean a better or cheaper listing?"
- "Which borough offers the best value — not just the cheapest price?"

These questions shaped how I interpreted each chart rather than just producing it.

🛠️ Tech Stack

Language: Python 3
Libraries: Pandas, NumPy, Matplotlib, Seaborn
Environment: Jupyter Notebook
Dataset: NYC Airbnb Listings 2024 via Zero Analyst / Kaggle


📁 Project Structure

NYC-Airbnb-EDA/

│
├── nyc_airbnb_eda.ipynb     # Full analysis notebook

├── dataset/
│   └── airbnb_nyc_2024.csv  # Source data (or link to download)

└── README.md

🚀 How to Run bash
# 1. Clone the repo
git clone https://github.com/qibbychan/NYC-Airbnb-EDA.git
cd NYC-Airbnb-EDA

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 3. Launch the notebook
jupyter notebook nyc_airbnb_eda.ipynb

📸 Sample Visualisations

Add screenshots of your best charts here — drag and drop into GitHub when editing.
Suggested visuals to include:

Room type distribution bar chart
Price by neighbourhood boxplot
Correlation heatmap
Availability vs price scatterplot



🔮 What I'd Do Next

 Connect this dataset to SQL for deeper aggregation queries
 Build an interactive Power BI dashboard for non-technical stakeholders
 Compare 2024 data with previous years to spot post-pandemic travel trends
 Apply a price prediction model using location and room type as features


🙏 Acknowledgements
Tutorial reference: Zero Analyst — NYC Airbnb EDA Project · Dataset: NYC Airbnb Listings 2024

🏷️ Topics
eda python data-analytics airbnb new-york-city pandas seaborn matplotlib data-cleaning data-visualization jupyter-notebook
