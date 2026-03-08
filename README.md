# International T20 Cricket Data Analysis

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Python](https://img.shields.io/badge/Python-3.x-green.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow.svg)

## Project Overview

This project is part of a **Data Science Fundamentals** assignment. The scenario simulates a role as a Data Scientist at the **International Cricket Council (ICC)**, joining the Analytics Team responsible for pre-match, live-match, and post-match analyses.

The primary goal of this project is to perform sanity checks, clean, and explore a comprehensive dataset containing historical T20 match data, followed by drawing key insights ranging from venue popularity to team win percentages and match scorecards.

## Dataset Description

- **Records**: 1417 T20 International Matches
- **Details**: Each row contains comprehensive data corresponding to a single T20 match, including details about innings, over-by-over deliveries, venues, match outcomes, and match conditions.
- **Source Format**: Initially parsed from structured text/JSON formats and analyzed in tabular format using Pandas.

## Key Objectives & Analyses Performed

1. **Data Cleaning & Preprocessing**:
   - Cleaned and renamed nested/messy column names (e.g., changing `meta.created` to `created_date`) into localized, readable formats.
   - Handled missing values (NaNs) and assessed data structure types for seamless processing.

2. **Exploratory Data Analysis (EDA) & Insights**:
   - **Venue Analysis**: Identified the **top 3 venues** globally that hosted the maximum number of T20 matches.
   - **Rivalry Analysis**: Discovered the pair of international cricket teams that have played the highest number of T20 matches against one another.
   - **Performance Tracking**: Calculated and visualized the **top 5 teams by win percentage** globally (Win % = Matches Won / Matches Played \* 100).

3. **Advanced Functionality - Scorecard Generation**:
   - Developed a custom scorecard generation function.
   - By parsing the deeply nested innings data, the function returns two robust DataFrames per match: detailing the top 4 run-scorers and the top 4 wicket-takers/bowlers for each participating team.

## Tech Stack

- **Language**: Python 3
- **Libraries**:
  - `NumPy` - Numerical operations and calculations.
  - `Pandas` - Core data manipulation, transformation, and analysis.
  - `Jupyter Notebook` / `Google Colab` - Interactive development environment.

## How to Run Locally

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Kingstar20524/dataScience-assignment-0.git
   ```
2. **Navigate to the directory**:
   ```bash
   cd Data-Science-Assignment-1
   ```
3. **Install Requirements**:
   Ensure you have `pandas` and `numpy` installed in your Python environment.
   ```bash
   pip install pandas numpy notebook
   ```
4. **Launch the Jupyter Notebook**:
   ```bash
   jupyter notebook International_T20_Data_Analysis.ipynb
   ```

_Alternatively, click on the **"Open In Colab"** badge inside the Notebook to run it directly in your browser without any local setup._

---

**Disclaimer**: This project was built for an academic assignment and analytics demonstration purposes based on historical T20 records.
**Acknowledgements**: Special thanks to the internet, YouTube tutorials, and rigorous self-study for making this project possible, filling in the gaps where formal university resources fell short.
