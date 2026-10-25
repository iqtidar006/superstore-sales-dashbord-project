# Superstore Sales Performance Dashboard

An interactive dashboard that shows how sales are performing, how they compare with the same months a year earlier, and which regions and product groups are driving the change.

**Live dashboard:** [https://iqtidar006.github.io/superstore-sales-dashbord-project/]

## What it shows
- Sales, orders, average order value and customers, each compared with the same months a year earlier
- Monthly sales chart with the previous year's line for comparison
- Sales by region (select a region to filter the whole page)
- Sortable sub-category performance table
- An automatic summary sentence naming the biggest gain and the biggest drop

## Data
The Superstore sales sample dataset: 9,800 order lines from 4,922 orders across four US regions, January 2015 to December 2018. Source: [WHERE YOU DOWNLOADED IT]. The dataset has no profit column, so the dashboard measures sales, orders and customers.

## How it works
- Python (pandas) cleans the data and converts it into a compact form embedded in the page
- Filters select the chosen months and the same months a year earlier, which removes the effect of seasonality
- Orders and customers are counted once each using unique IDs; average order value is sales divided by orders
- Charts are drawn as SVG with plain JavaScript, with no chart libraries

## Built with
Python (pandas), HTML, CSS, JavaScript, SVG. Tested in headless Chromium with Playwright.
## Run it locally
Download `index.html` and open it in any browser.
