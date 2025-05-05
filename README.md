# Monthly Email Sending Activity by Account

This project analyzes monthly email-sending behavior across user accounts. It calculates each account's contribution to the total email volume for a given month and identifies their first and last email send dates.

## Key Insights

- **Percentage of Emails Sent per Account per Month**  
- **First and Last Email Dates** per account in each month  
- **Monthly Trends in Email Activity** across all users  

## How It Works

The query uses:
- **Window functions** to compute rolling metrics like count, min, and max dates  
- **Date manipulation** (via `DATE_ADD` and `DATE_TRUNC`) to align data by calendar month  
- **Deduplication** (`DISTINCT`) to ensure clean output per account-month pair

## Use Cases

- Monitoring **email campaign reach per user**  
- Understanding **user re-engagement cycles**  
- Identifying **inactivity periods**  
- Supporting segmentation and retention analysis
