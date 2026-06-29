# MT Global Chargeback Dashboard

Live dashboard for MT Global chargebacks, pulling data straight from Google Sheets.

**Live link:** https://mt-global-co.github.io/Chargeback-Dashboard/

## What's inside
- **Overview tab** — total chargebacks, win % / loss %, number still in review, and total value, plus status/reason charts and a ranked "top reasons" table.
- **Chargeback Details tab** — searchable, sortable, filterable table of Status, Order #, Total Chargeback amount, and Reason for Chargeback.
- **Rapid Dispute Resolution tab** — RDR cases from the `RDR` sheet: count, total value, average per case, and a searchable/sortable table.
- **Refresh data** button pulls the latest rows live from the Google Sheet (same as the MT Global Dashboard).
- Always-on dark theme.

## Data source
Reads the published Google Sheet:
`https://docs.google.com/spreadsheets/d/1TuMaYXN1aJnW5Ms2ioHj1AqHOV7Uy8OGZ4TiP_CZgQE`

The sheet must be shared as **"Anyone with the link can view"**. Two tabs are read:
- **first sheet** — the main chargebacks (Overview + Chargeback Details tabs)
- **`RDR`** — Rapid Dispute Resolution cases (RDR tab)

Both use the same columns: `Status | Order Number | Total Chargeback | Reason for Chargeback | Notes`

Status values are matched loosely: anything containing "won", "lost", "review", or "resolved" is bucketed accordingly.

## Updating
Just edit the Google Sheet. Open the dashboard and click **Refresh data** — no redeploy needed.
