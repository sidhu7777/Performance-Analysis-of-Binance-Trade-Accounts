#  Performance Analysis of Binance Trade Accounts

This project presents a comprehensive analysis of trading performance across Binance accounts over a 90-day period. Conducted as part of an internship at **Primetrade.ai**, the goal was to assess, compare, and rank accounts using key financial metrics and optimization techniques.

##  Project Overview

The analysis focuses on:

- Cleaning and structuring raw trade history data
- Engineering relevant features for deeper insight
- Calculating financial metrics like:
  - Profit & Loss (PnL)
  - Return on Investment (ROI)
  - Win Rate
  - Maximum Drawdown (MDD)
  - Sharpe Ratio
- Visualizing key trading patterns and performance trends
- Ranking accounts through a custom scoring system using:
  - Manual weight assignment
  - Bayesian Optimization for weight tuning

##  Financial Metrics Used

| Metric         | Description |
|----------------|-------------|
| **PnL**        | Total realized profit per account |
| **ROI**        | Profitability relative to total capital traded |
| **Win Rate**   | Percentage of profitable trades |
| **MDD**        | Maximum peak-to-trough loss |
| **Sharpe Ratio** | Risk-adjusted return measure |

##  Visual Insights

The notebook includes various visualizations such as:

- Distribution of trade prices
- Cumulative PnL over time
- Profit vs. loss trade counts
- Trading activity by hour
- Best and worst performing assets

##  Ranking Methodology

A scoring algorithm was developed using a weighted combination of the metrics. Two ranking strategies were implemented:

1. **Manual Weighting**  
   - PnL: 45%  
   - ROI: 28%  
   - Win Rate: 22%  
   - Sharpe Ratio: 15%  
   - MDD: -10% (penalty for higher drawdowns)

2. **Bayesian Optimization**  
   - Automatically fine-tunes the weights to maximize ranking quality based on data.

The final scores were used to rank and select the **Top 20 Performing Accounts**.


##  Tech Stack

- **Python**: pandas, numpy, matplotlib, seaborn
- **Optimization**: scikit-optimize
- **Jupyter Notebook**: for analysis and presentation

## Outcomes

- Built a modular, data-driven pipeline for trade performance analysis.
- Delivered insights into profitability, consistency, and risk across accounts.
- Applied Bayesian Optimization to remove subjectivity in scoring.
- Produced a ranked list of high-performing accounts based on multiple metrics.



---

**Developed For the Assignment at  [Primetrade.ai](https://primetrade.ai)**  
**About Me**  
I'm **Vineeth Raja Banala**, a Data Science graduate passionate about turning raw data into actionable insights. With hands-on experience in Python, data analysis, and machine learning, I enjoy building real-world data-driven solutions that are both structured and scalable. 




