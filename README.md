# NorthWestern Energy Wizard

Browser-based dashboard for exploring NorthWestern Energy AMI usage exports for electric-only residential analysis.

## What It Does

Open `index.html` in a browser, upload a NorthWestern detailed usage CSV, and explore:

- daily heatmap with days on the x-axis and hour of day on the y-axis
- typical day load shape with `All days`, `Weekdays`, and `Weekends` toggles
- day-of-week comparison with season and month filters
- monthly totals
- peak hour timing with season and month filters
- monthly always-on vs. active-use breakdown
- savings opportunity recommendations based on the uploaded interval data

## Input Requirements

The dashboard is built for the direct NorthWestern hourly export and works without modification when the CSV includes these columns:

- `DATE`
- `START TIME`
- `USAGE`

The page trims larger files to the most recent `8,760` hourly reads.

## How To Use It

1. Open `index.html` in a modern web browser.
2. Drag in your NorthWestern detailed usage CSV, or use the upload button.
3. Review the charts and use the month, season, and series filters to explore your patterns.

## How To Get Your Data

NorthWestern explains the detailed usage export here:  
https://www.northwesternenergy.com/create-manage-account/detailed-energy-usage

My Energy Account login:  
https://myaccount.northwesternenergy.com/NWESSP/Index.aspx

Basic steps:

1. Log in to My Energy Account.
2. Select `Billing` from the menu.
3. Click `View Detailed Usage`.
4. Choose the time resolution and time period you want.
5. Download the file using the export button in the portal.

## Privacy

Your CSV is processed locally in the browser and is not uploaded by the dashboard.

## Hosting

This repo can be hosted directly with GitHub Pages because the dashboard is a single self-contained `index.html` file.

Live site:  
https://natphi.github.io/NWE_Viz/
