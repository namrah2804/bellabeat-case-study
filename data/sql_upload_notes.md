# SQL Upload Notes (Prepare)

## SQL Environment
- Platform: Microsoft SQL Server
- Tool: SQL Server Management Studio (SSMS)

## Database
- Database name: BellabeatFitbit
- Schema: dbo

## Tables Created (raw imports)
Two export folders were imported as separate tables to avoid mixing time windows before processing.

- dbo.daily_activity_0312_0411
- dbo.daily_activity_0412_0509
- dbo.sleep_day_0312_0411 (only if available)
- dbo.sleep_day_0412_0509 (only if available)
- dbo.weight_log_0312_0411 (optional)
- dbo.weight_log_0412_0509 (optional)

## Import Method
CSV files were imported using the SSMS Import Data wizard. No cleaning, joins, or transformations were applied at this stage.
