# MT Global Chargeback Dashboard

Live dashboard for MT Global chargebacks, pulling data straight from Google Sheets.

**Live link:** https://connectwithpier.github.io/MT-Global-Chargeback-Dashboard/

## What's inside
- **Overview tab** — total chargebacks, win % / loss %, number still in review, and total value, plus status and reason charts.
- **Chargeback Details tab** — searchable, sortable, filterable table of Status, Order #, Total Chargeback amount, and Reason for Chargeback.
- **Refresh data** button pulls the latest rows live from the Google Sheet (same as the MT Global Dashboard).

## Data source
Reads the published Google Sheet:
`https://docs.google.com/spreadsheets/d/1TuMaYXN1aJnW5Ms2ioHj1AqHOV7Uy8OGZ4TiP_CZgQE`

The sheet must be shared as **"Anyone with the link can view"**. Expected columns:
`Status | Order Number | Total Chargeback | Reason for Chargeback | Notes`

Status values are matched loosely: anything containing "won", "lost", or "review" is bucketed accordingly.

## Updating
Just edit the Google Sheet. Open the dashboard and click **Refresh data** — no redeploy needed.
