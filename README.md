cat > README.md << 'EOF'
# Restaurant Tipping Analysis

## Overview
Exploratory Data Analysis (EDA) of restaurant tipping patterns using Python, pandas, matplotlib, and seaborn.

## Project Description
This project analyzes a dataset of 244 restaurant transactions to understand tipping behavior patterns. The analysis includes:

- Data loading and exploration
- Feature engineering (tip rate, bill per person, tip per person, large party indicator)
- Statistical visualizations (box plots, scatter plots, histograms)
- Homoscedasticity assessment between tip rate and party size
- Subgroup analysis (smokers vs non-smokers)

## Technologies Used
- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **matplotlib** - Data visualization
- **seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive development environment

## Dataset
The dataset contains 244 restaurant transaction records with the following features:
- `total_bill` - Total bill amount before tip
- `tip` - Tip amount
- `sex` - Gender of server
- `smoker` - Whether party included smokers
- `day` - Day of the week
- `time` - Lunch or dinner
- `size` - Party size

## Key Findings
- Strong positive correlation between total bill and tip amount
- Heteroscedasticity observed: small parties (2-3) show high variability in tip rates (5-35%), while large parties (4+) tip more consistently (12-18%)
- Smoker subset shows similar patterns but with increased variance
- Tip rates do not follow the theoretical reference line (0.18 - 0.1 × size)

## Engineered Features
- **tip_rate** - Ratio of tip to total bill
- **bill_per_person** - Total bill divided by party size
- **tip_per_person** - Tip divided by party size
- **is_large_party** - Boolean for party size ≥ 4
- **total_cost** - Sum of total bill and tip

## Files
- `COMP333_LA1_Analysis.ipynb` - Main Jupyter notebook with complete analysis
- `COMP333_LA1_Analysis.html` - HTML export with all visualizations
- `tips.csv` - Dataset (244 rows × 7 columns)

## How to Run
1. Clone this repository:
```bash
   git clone https://github.com/MoeSartawi/Restaurant-Tipping-Analysis.git
   cd Restaurant-Tipping-Analysis
```

2. Install required packages:
```bash
   pip install pandas numpy matplotlib seaborn jupyter
```

3. Launch Jupyter Notebook:
```bash
   jupyter notebook COMP333_LA1_Analysis.ipynb
```

4. Run all cells: **Kernel** → **Restart & Run All**

## Course Information
- **Course:** COMP 333 - Data Analysis
- **Assignment:** Lab Assignment 1 - Exploratory Data Analysis
- **Institution:** Concordia University
- **Date:** February 2026

## Author
**Mohammad Salah**  
