# Accounts Payable Aging Analysis

## Overview
A multi-sheet Accounts Payable analysis built from raw bill/transaction data across multiple business entities. The workbook takes a flat transaction export and turns it into entity-level, vendor-level, and aging-bucket summaries using pivot tables.

## Dataset
`Combined AP Data` — 460+ AP transactions across 5 entities, with vendor, due date, days past due, aging bucket, and open balance fields.

## What's in the workbook

| Sheet | Purpose |
|---|---|
| Combined AP Data | Raw transaction-level data (source) |
| Entity Summary | Total payable, open balance, % of AP, and past-due counts by entity |
| Aging Analysis | Aging bucket breakdown (Current / 1-30 / 31-60 / 61-90 / 91+ days) by entity, with % over 90 days |
| Vendor Analysis | Spend and balance breakdown by vendor |
| Entity Aging | Aging detail per entity |
| Top Vendors | Top 15 vendors by open balance, with a filterable chart |

## Key techniques used
- Pivot tables summarizing transaction-level data by entity, vendor, and aging bucket
- Calculated fields (% of AP, % over 90 days)
- Slicers/filters for interactive vendor analysis
- Cross-sheet pivot table relationships built off a single source table

## Screenshots

**Accounts Payable by Entity**
![Entity Summary](./screenshots/entity-summary.png)

**Aging Analysis by Entity**
![Aging Analysis](./screenshots/aging-analysis.png)

**Top 15 Vendors by Open Balance**
![Top Vendors](./screenshots/top-vendors.png)

## File
[`Combined_AP_Report.xlsx`](./Combined_AP_Report.xlsx)
