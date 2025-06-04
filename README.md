# Lavpop Reports

This project contains the HTML dashboard and data tables for the Lavpop reporting website.

## Configuration

Connection details for the data tables (the Google Apps Script URL and Drive file IDs) are stored in `config.js` so the HTML remains generic. To point the dashboard to your own files:

1. Open `config.js`.
2. Replace the `scriptUrl` value with the URL of your deployed Apps Script web app.
3. Update the `fileIds` object with the IDs of your CSV files or Google Sheets.

After editing `config.js`, reload the HTML pages and the new sources will be used.
