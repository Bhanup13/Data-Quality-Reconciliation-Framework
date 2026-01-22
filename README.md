# Data-Quality-Reconciliation-Framework

## Overview
A lightweight framework to validate data quality during ETL runs and generate a simple audit report.
Built as a learning project and later reused as a pattern in batch pipelines.

## Problem Statement
ETL pipelines can succeed technically but still deliver incorrect data (missing records, duplicates, null spikes).
This project adds checks that catch issues early and produce a clear report.

## Checks Included
- Row count reconciliation (source vs target)
- Null checks for critical columns
- Duplicate key checks
- Threshold checks (unexpected spikes/drops)

## Tech Stack
- Python
- SQL
- (Optional) Great Expectations
- Output report: CSV / JSON
- ## How It Works
1. Run checks after each load step
2. Store results in a report file
3. Fail the pipeline if critical checks fail

## Outcome
- Faster detection of bad loads
- Easier troubleshooting with audit output.
