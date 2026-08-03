# Fashion Trend Radar

A live data pipeline tracking rising fashion micro-trends and Gen Z quality/values 
signals, built to help brands catch trend changes before competitors do.

## Live Dashboards

🔗 **[View Live Interactive Dashboard on Tableau Public](https://public.tableau.com/app/profile/khushi.chandel/viz/Fashion_Trend_Radar/Dashboard1?publish=yes)** — Explore the interactive dashboard directly in your browser; no installation required.

💻 **Power BI Desktop:** `Fashion_Trend_Radar_Dashboard.pbix` — Connects to this repository's latest dataset and can be refreshed on open (requires Power BI Desktop).
## Business Problem
Fast fashion brands often react to micro-trends 3-6 months too late, and may be 
missing a broader quality/trust gap that erodes customer confidence.

## Business Question
Which rising micro-trends are brands currently under-reacting to, and does 
customer sentiment reveal quality gaps brands are missing?

## Data Sources
- **Google Trends API** (via pytrends) — live search interest data, US vs India comparison
- **Women's E-Commerce Clothing Reviews** (Kaggle) — 22,000+ real customer reviews for sentiment analysis

## Tech Stack
- **Python** — data collection, cleaning, correlation analysis, sentiment analysis (TextBlob, NLTK)
- **SQL** (SQLite) — data querying and validation
- **Excel** — pivot table analysis and visualization
- **Power BI** — interactive dashboard, connected live to GitHub-hosted data
- **Tableau Public** — published interactive dashboard
- **GitHub Actions** — fully automated daily data refresh (retry logic for API rate-limiting)

## Key Findings
1. **Trend divergence:** US and India fashion trends don't simply follow the same 
   timeline — cottagecore shows sustained US interest while India shows minimal 
   engagement, suggesting some trends emerge independently rather than following 
   a predictable delay.
2. **Quality over values:** The "Trend" clothing category shows the lowest customer 
   sentiment (0.20 vs ~0.25 elsewhere). Analysis of negative reviews reveals the 
   driver is fit/fabric quality inconsistency, not values-based concerns — 
   suggesting brands chasing trend speed risk measurable quality-driven trust erosion.

## Automation
This pipeline runs daily via GitHub Actions, pulling fresh Google Trends data and 
committing it automatically — verifiable in the commit history. Includes retry 
logic to handle API rate-limiting gracefully.

## Status
✅ Complete — Python, SQL, Excel, sentiment analysis, Power BI, and Tableau Public 
dashboard all built and functioning.
