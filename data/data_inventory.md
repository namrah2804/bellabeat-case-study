# Data Inventory 

## Download
- Dataset: FitBit Fitness Tracker Data
- Source: Kaggle (Mobius)
- License: CC0 (Public Domain)
- Download format: ZIP file

## ZIP Contents
The ZIP file contained two export folders:
- mturkfitbit_export_3.12.16-4.11.16
- mturkfitbit_export_4.12.16-5.12.16

## Selected Files for Analysis and Purpose
This document explains why specific datasets from the Fitbit Fitness Tracker Data were selected for analysis and how each file supports the Bellabeat business questions. Files were chosen based on relevance to marketing-focused insights rather than data availability alone.
- dailyActivity_merged.csv (both exports)
- sleepDay_merged.csv (available in one export)
- weightLogInfo_merged.csv (optional)

## Rationale
Daily activity data provides the strongest basis for analysing smart device usage trends. Sleep data was included where available to add wellness context. Weight data was reviewed but treated as optional due to sparse logging.


### dailyActivity_merged.csv (Primary Dataset)
**Why this file was selected:**
- Contains daily steps, distance, activity minutes, sedentary time, and calories burned.
- Provides a complete daily view of user engagement with smart devices.
- Suitable for identifying high-level usage trends such as activity intensity, consistency, and weekday versus weekend behaviour.

**Business questions supported:**
- How do users engage with smart devices on a daily basis?
- What activity and calorie-burning patterns are most common?
- How can activity trends inform Bellabeat’s movement-focused messaging?

---

### sleepDay_merged.csv (Secondary Dataset – Partial Coverage)
**Why this file was selected:**
- Sleep is a core component of holistic wellness, which aligns with Bellabeat’s brand positioning.
- Enables exploration of the relationship between activity and recovery where sleep data is available.
- Included despite incomplete coverage to provide additional wellness context rather than full population inference.

**Business questions supported:**
- How does sleep behaviour relate to daily activity levels?
- Can Bellabeat position sleep insights as part of a balanced wellness narrative?

---

### weightLogInfo_merged.csv (Optional / Contextual)
**Why this file was reviewed:**
- Represents deeper user engagement with personal health tracking.
- Helps assess how frequently users log sensitive health metrics.

**Limitations:**
- Data is sparse and inconsistent across users.
- Not required to answer core business questions and therefore treated as optional.

---

## Files Excluded from Analysis

### Minute-Level Activity and Sleep Files
These datasets were excluded because:
- They are highly granular and not necessary, to keep the work aligned with the marketing-focused business questions and to prioritise interpretable daily trends for non-technical stakeholders
- Daily-level summaries are more appropriate for stakeholder communication and strategic insights.

 Minute-level analysis can be added later to explore time-of-day engagement and wear-time patterns.

### Redundant Daily Files (Steps-only, Calories-only)
These were excluded because their information is already included in `dailyActivity_merged.csv`, making them unnecessary duplicates.

---


