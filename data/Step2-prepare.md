## Step 2 – Prepare

### 2.1 Data sources

The primary dataset for this case study is the **Fitbit Fitness Tracker Data** (CC0: Public Domain) made available on Kaggle by Mobius. It contains personal fitness tracker data from 30 Fitbit users, including minute‑level and daily‑level records for physical activity, steps, calories, heart rate, and sleep monitoring. This data is used to explore smart‑device usage patterns and daily habits.  

At this stage, the Fitbit dataset is the only data source. It serves as a proxy for Bellabeat customers’ behaviour because it provides real smart‑device usage data that is publicly available and free to use for learning purposes.

---

### 2.2 Storage and organisation

Downloaded Fitbit CSV files are stored in the `data/raw/` folder of this repository. Raw files from Kaggle are kept unchanged so that the original data is always available. Any cleaned or aggregated tables created during later steps will be saved in `data/processed/`. Separating raw and processed data helps preserve data integrity and makes the workflow reproducible.

-----

### 2.3 Data structure

Each CSV file represents a different aspect of usage (for example, daily activity, daily calories, daily steps, and sleep). Most of the daily‑level tables are stored in **wide** format, with one row per user per date and separate columns for different measures (such as total steps, total distance, sedentary minutes, and very active minutes). Some other tables, such as minute‑level data, are closer to **long** format, with multiple rows per user per day.


----

### 2.4 Credibility, bias, and limitations

The Fitbit dataset is publicly shared under a CC0 licence and comes from real users, so it is suitable for learning and exploratory analysis. However, it has important limitations:

- Only 30 users are included, so the sample size is small.  
- Users are self‑selected Fitbit owners and may not represent Bellabeat’s target population.  
- The time period is limited and may miss seasonal or long‑term trends.  
- The data is from Fitbit devices, not from Bellabeat products directly, and contains very little demographic information.

Because of these constraints, the dataset is considered directional rather than fully representative. Insights will be used to generate ideas about smart‑device usage patterns, but they should not be treated as definitive descriptions of all Bellabeat customers.

