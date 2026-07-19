# Fashion Trend Radar

A live data pipeline tracking rising fashion micro-trends and Gen Z values-shift signals, built to help brands catch trend changes before competitors do.

## Business Problem
Fast fashion brands often react to micro-trends 3-6 months too late, and are missing a broader values shift — Gen Z increasingly chooses brands based on trust, cruelty-free ethics, and quality, not just trend-following.

## Business Question
Which rising micro-trends are brands currently ignoring, and are they missing the Gen Z values shift?

## Data Sources
- **Google Trends API** (via pytrends) — live search interest data, US vs India comparison
- **Reddit** — community discussion data for sentiment/values analysis

## Tech Stack
- Python (data collection, cleaning, correlation analysis)
- SQL (data querying)
- Excel (initial exploration)
- Power BI (interactive dashboard)
- GitHub Actions (automated daily data refresh)

## Key Finding (so far)
US and India fashion trends don't simply follow the same timeline — for
keywords like "cottagecore," India shows almost no engagement for months
while the US sustains strong interest, suggesting some trends may emerge
independently rather than following a predictable delay.

## Status
🚧 In active development — Python analysis complete, SQL/Power BI/Excel in progress.
