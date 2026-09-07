# Data Analyst Job Market Analysis

## Overview
What skills should a data analyst actually learn to get hired? This project
analyzes **196,075 real "Data Analyst" job postings** (scraped from Google
Search results, sourced from Luke Barousse's open dataset) to answer that
question with data instead of guesswork — what skills are most in demand,
which ones pay the most, and how remote-friendly the role really is.

## Data Source
- **Dataset:** `lukebarousse/data_jobs` (same data behind Kaggle's
  "Data Analyst Job Postings [Pay, Skills, Benefits]"), loaded directly via
  Hugging Face Datasets
- **785,741 total postings** across all data roles; filtered down to
  **196,075 Data Analyst postings**
- Covers job title, location, country, remote-work flag, posted date,
  salary (where disclosed), and parsed required skills per posting

## Analysis Performed
1. **Top in-demand skills** — ranked the 15 most-requested skills across
   all Data Analyst postings
2. **Skill category breakdown** — grouped skills into categories
   (analyst tools, programming, cloud, databases, libraries, etc.) to see
   which category of skill matters most
3. **Salary by skill** — for the 10 most in-demand skills, compared average
   yearly salary (where postings disclosed pay)
4. **Remote vs on-site** — what share of Data Analyst postings are remote
5. **Postings over time** — how hiring volume moved month to month across 2023
6. **Top hiring countries** — which countries post the most Data Analyst roles

## Key Findings
- **SQL is the single most in-demand skill**, appearing in 92,428 postings
  (~47% of all Data Analyst postings) — well ahead of Excel and Python.
- **"Analyst tools" (Excel, Tableau, Power BI, SAP, etc.) and "programming"
  are by far the two largest skill categories**, together accounting for the
  vast majority of skill mentions — confirming that both spreadsheet/BI
  tools and coding are considered essential, not optional, for this role.
- Among the 10 most in-demand skills, **Python commands the highest average
  salary (~$101,457/yr)**, while more document-oriented tools like Word sit
  at the lower end (~$82,617/yr) — suggesting that programming ability, not
  just tool familiarity, is what employers pay a premium for.
- **Only 6.8% of Data Analyst postings are remote** — the vast majority
  (93.2%) are on-site or hybrid, a useful reality check against the
  "remote-friendly by default" assumption around data roles.
- **The United States dominates hiring volume** (67,816 postings), followed
  by France, the UK, Germany, and Singapore.
- Job-posting volume shows a **notable dip mid-year (April–May) and a spike
  in August 2023**, hinting at seasonal hiring cycles worth watching.
- **Caveat:** only ~2.8% of postings (5,451) disclosed a salary figure, so
  the salary findings, while directionally useful, are based on a small,
  possibly non-representative subset of listings.

## Tech Stack
Python, Pandas, Matplotlib, Seaborn, Hugging Face Datasets

## Files in this Repo
- `Data_Analyst_Job_Market_Analysis.ipynb` — full analysis notebook
- `outputs/data_analyst_jobs_clean.csv` — cleaned, filtered dataset used for analysis
- `outputs/*.png` — the 6 charts (top skills, skill categories, salary by
  skill, remote vs on-site, postings over time, top countries)

## Author
Sahil Kumar — [GitHub](https://github.com/sahilkumar620) ·
[Portfolio](https://sahilkumar620.github.io/SAHIL-PROTFOLIO/)
