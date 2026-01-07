# Data Organisation (Prepare)

## Data Format
Most datasets are in long format, where each row represents a single user record for a specific date.

## Key Identifiers
- Id: unique user identifier
- Date fields vary by file:
  - dailyActivity_merged: ActivityDate
  - sleepDay_merged: SleepDay
  - weightLogInfo_merged: Date

## Joins
Datasets can be joined using the user Id and date fields once date formats are standardised in the Process step.

## Notes
Date formats are inconsistent across files and will be addressed during data processing.
