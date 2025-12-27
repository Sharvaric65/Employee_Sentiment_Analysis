# Employee Sentiment Analysis

## Project Overview
This project analyzes unlabeled employee messages to assess sentiment, engagement, and potential flight risks using NLP and statistical techniques.

## Dataset
- File: test.csv
- Data contains employee messages with timestamps and sender information.

## Methodology
1. Sentiment labeling using VADER sentiment analyzer.
2. Exploratory Data Analysis to understand sentiment trends.
3. Monthly sentiment scoring per employee.
4. Employee ranking based on sentiment scores.
5. Flight risk identification using a rolling 30-day window.
6. Linear regression modeling to analyze sentiment trends.

## Sentiment Scoring
- Positive: +1  
- Negative: -1  
- Neutral: 0  

Scores reset every month.

## Flight Risk Criteria
An employee is flagged as a flight risk if they send 4 or more negative messages within any rolling 30-day period.

## Predictive Model
A linear regression model was trained using:
- Message count per month
- Average message length

Model performance was evaluated using MSE and R² score.

## Key Outputs
- Top 3 positive and negative employees per month
- List of flight risk employees
- Visualizations showing sentiment distribution and trends

## How to Run
1. Open the notebook `Employee_Sentiment_Analysis.ipynb`
2. Ensure `test.csv` is in the same directory
3. Run all cells from top to bottom
