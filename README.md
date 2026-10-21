# Sales & Finance Intelligence Dashboard (HTML/CSS/JS only)

No Python, no Node, no install. Double-click `index.html`. It needs an internet connection once to load the chart library (Chart.js from cdnjs) and the font.

Demo mode uses clearly labelled synthetic data. **There is no Salesforce or SAP connection.** Everything runs in the browser; nothing is sent anywhere.

## Use
- Pages: Executive overview, Salesforce sales analytics, Data connections. Filters: period and region.
- **Import CSV** loads your own data in the browser only. Columns: `date, region, product, customer, rep, revenue, cogs` (date as YYYY-MM-DD). See `sample_data.csv`. **Reset demo data** restores the demo.

## Publish on GitHub Pages
Push these files to a repository, then Settings > Pages > deploy from the main branch, root folder.

## Metrics
Booked revenue = revenue in period. Gross profit = revenue - COGS. Margin = GP / revenue. Target achievement = booked / (monthly target x months). Win rate = won / (won + lost). Retention = prior-period customers who bought again / prior-period customers. Pipeline is forecast, never added to booked revenue.
Modelled in demo mode only: budget, target, leads, lost deals, pipeline, receivables, aging.

## Not included
SAP, Operations and Detailed Analysis pages; XLSX import; export; login and roles; real Salesforce/SAP connections (these need a server, so they cannot be done securely in a browser-only app).
