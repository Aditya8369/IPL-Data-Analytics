# IPL Data Analytics (2008–2026)

Exploratory data analysis of Indian Premier League (IPL) match data spanning every season from 2008 to 2026 — covering team performance, toss trends, scoring patterns, venues, and player awards.

## Project Description

This project analyzes 1,243 IPL matches to uncover patterns in:

- Match volume and trends across 19 seasons
- Team performance — total wins and win percentage
- Toss decisions (bat vs. field) and their impact on match outcomes
- Team innings scoring distribution
- Most-used venues
- "Player of the Match" award leaders
- Winning margins (by runs vs. by wickets)

The analysis handles real-world data quirks such as franchise renames (e.g. Delhi Daredevils → Delhi Capitals, Kings XI Punjab → Punjab Kings) and missing values in tied or no-result matches.

## Dataset

- **File:** `IPL_Matches_Data_2008_2026.csv`
- **Link:** https://www.kaggle.com/datasets/arjunsinghgangwar/ipl-20082026-matches-dataset
- **Rows / Columns:** 1,243 matches × 31 fields
- **Fields include:** season, date, city, venue, teams, toss winner/decision, innings scores and wickets, match winner, result type, win margin, player of the match, umpires, and playing XI for both teams.
- **Source:** Provided as a course/project dataset (place the CSV in the project root before running the notebook). If you are sourcing your own copy, IPL ball-by-ball and match-summary datasets of this shape are commonly published on [Kaggle](https://www.kaggle.com/datasets?search=ipl).

## Technologies Used

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| pandas, numpy | Data cleaning & analysis |
| matplotlib, seaborn | Data visualization |
| Jupyter Notebook | Interactive analysis environment |

## Project Structure

```
├── IPL_Data_Analytics.ipynb                # Main analysis notebook (code + charts + narrative)
├── IPL_Matches_Data_2008_2026.csv          # Source dataset
├── requirements.txt                        # Python dependencies
├── IPL_Project_Report.docx                 # Full project documentation
└── README.md                               # Overview of project
```

## Setup & Run Instructions (for Windows)

1. **Clone/download the project files** into a single folder, including the CSV dataset.
2. **Create a virtual environment (recommended):**
   ```bash
   python -m venv venv
   venv\Scripts\activate      
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Launch Jupyter and run the notebook:**
   ```bash
   jupyter notebook IPL_Data_Analytics.ipynb
   ```
   Then run all cells (`Cell → Run All` or `Kernel → Restart & Run All`).
5. Ensure `IPL_Matches_Data_2008_2026.csv` is in the same directory as the notebook, or update the `DATA_PATH` variable in the first code cell.

## Key Findings

- Mumbai Indians and Chennai Super Kings lead the league in total match wins across IPL history.
- Gujarat Titans post the highest win percentage among teams with a substantial number of matches played.
- Captains winning the toss choose to field first roughly two-thirds of the time, and chasing teams win marginally more often than teams batting first.
- Eden Gardens is among the most-used venues, reflecting long-tenured host franchises.
- AB de Villiers holds the most "Player of the Match" awards in the dataset.

## Author

Aditya Mahajan (PVPIT, Pune)
