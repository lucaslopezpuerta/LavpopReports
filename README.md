# Lavpop Analytics Dashboard

This repository hosts the static files for the **Lavpop Analytics Dashboard**. It provides interactive charts and tables that summarize laundromat performance.

## Opening the dashboard

1. **index.html** – main dashboard with interactive charts. Open this file in any modern web browser.
2. **data-tables.html** – companion page with sortable and exportable tables. Also open in a browser.

## Dependencies

The dashboard relies on external libraries loaded from public CDNs:

- `index.html` uses [Google Charts](https://developers.google.com/chart) via `https://www.gstatic.com/charts/loader.js`.
- `data-tables.html` uses the DataTables jQuery plugin and extensions:
  - jQuery
  - DataTables core and Buttons extension
  - JSZip and pdfmake for export features

These libraries are referenced directly in each HTML file, so no additional installation is required.

## Updating the `charts/` directory

Chart HTML files are stored in the `charts/` folder. They are generated using the Google Apps Script found in `charts/Analytics Chart Generator.txt`. Run that script with updated analytics data to produce new chart files. Replace or add the resulting `.html` files inside `charts/` and commit the changes so the dashboard loads the latest charts.

## Contact
This project contains the HTML dashboard and data tables for the Lavpop reporting website. Questions about this report? Contact **Gabrielle Vilanova** or **Lucas López** at [lavpop.caxias@outlook.com](mailto:lavpop.caxias@outlook.com).

## Configuration

Connection details for the data tables (the Google Apps Script URL and Drive file IDs) are stored in `config.js` so the HTML remains generic. To point the dashboard to your own files:

1. Open `config.js`.
2. Replace the `scriptUrl` value with the URL of your deployed Apps Script web app.
3. Update the `fileIds` object with the IDs of your CSV files or Google Sheets.

After editing `config.js`, reload the HTML pages and the new sources will be used.
=======
