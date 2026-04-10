# NBA Player Salary ROI Analysis
## 1. Problem & User
  Target User: NBA Team General Managers (GMs) and Sports Analysts.
  Business Problem: NBA teams operate under a strict salary cap system. This data product helps decision-makers evaluate player contract efficiency by comparing salary investment with on-court performance, identifying high-value contracts and low-return contracts to support salary cap allocation.

## 2. Data
- Source: Simulated dataset based on real 2023–2024 NBA regular season statistics (consistent with standard ESPN and Kaggle datasets).
- Access Date: April 2024
- Key Fields: Player Name, Points Per Game (PPG), Salary (raw string with currency symbols)

## 3. Methods
1. Data Construction: Built a targeted sample including supermax players, rookie-scale players, and typical high-salary/low-production players.
2. Data Cleaning: Removed `$` and `,` symbols from salary strings using Python `str.replace()`, then converted values to integer type for calculation.
3. Metric Creation: Calculated `Cost_Per_Point` (salary divided by PPG) to measure financial efficiency.
4. Analysis & Visualization: Created a scatter plot to show performance (PPG) vs. salary, with a $40M supermax reference line for comparison.

## 4. Key Findings
- Lowest Efficiency Contract: Ben Simmons has extremely low ROI, earning approximately $38M with only 6.1 PPG.
- Highest Value Contract: Tyrese Maxey provides elite performance (25.9 PPG) on a cost-effective rookie contract ($4.3M), showing optimal investment efficiency.
- Justified Supermax Players: Stephen Curry, Joel Embiid, and Luka Doncic justify their $40M+ salaries with high baseline production.
- Efficiency Pattern: Higher salary does not guarantee higher performance; contract value depends heavily on production per dollar.

## 5. How to run
1. Download `ACC102_Notebook_NBA_ROI.ipynb`
2. Run in a standard Jupyter Notebook environment
3. Required libraries: `pandas`, `matplotlib`
4. The notebook generates a local sample dataset automatically; no external data download is required.

## 6. Product link / Demo
🎥 Demo Video: [Your 1–3 minute video link here]

## 7. Limitations & next steps
- Limitations: Analysis uses only Points Per Game (PPG), which does not reflect defensive contribution, playmaking (assists/rebounds), leadership, or off-court commercial value.
- Next Steps: Integrate advanced metrics such as Player Efficiency Rating (PER), Win Shares, or VORP to build a comprehensive multi-dimensional evaluation model. Expand the dataset to include more players and position-specific benchmarks.
