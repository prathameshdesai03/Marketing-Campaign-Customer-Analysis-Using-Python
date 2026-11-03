# Marketing Campaign Customer Analysis

## Project description (approximately 100 words)

This project analyzes customer demographics, purchasing behaviour, and marketing campaign responses using Python. It starts by cleaning the dataset, handling missing income values, converting date and categorical fields, and checking for outliers with the IQR and Z-score methods. It then uses descriptive statistics and correlation analysis to explore customer characteristics and spending patterns. New features summarize each customer's total product spending and purchase activity. Statistical inference estimates a 95% confidence interval, while regression examines the relationship between spending and purchase activity. Visualizations show income distribution, spending outliers, campaign responses, income versus spending, and customer acquisition trends. The findings can help guide customer segmentation and campaign planning.

## Files

- `marketing_campaign_analysis.py` — complete Python source code.
- `README.md` — project overview and instructions.
- `marketing_campaign.csv` — input dataset (not included; provide your own copy).

## Requirements

Python 3.9 or later is recommended.

Install the required libraries:

```bash
pip install pandas numpy scipy matplotlib seaborn scikit-learn
```

## Dataset

Place `marketing_campaign.csv` in the same folder as the Python script, or provide its location when running the script.

The script expects commonly used columns from the Marketing Campaign dataset, including `Income`, `Dt_Customer`, `Education`, `Marital_Status`, product spending columns (`MntWines`, `MntFruits`, `MntMeatProducts`, `MntFishProducts`, `MntSweetProducts`, `MntGoldProds`), purchase-count columns, campaign acceptance columns, and `Response`.

## Run the project

```bash
python marketing_campaign_analysis.py
```

Or specify a dataset and output folder:

```bash
python marketing_campaign_analysis.py --data path/to/marketing_campaign.csv --output results
```

The script prints statistical summaries and saves generated charts and CSV summaries in the output folder.

## Main analysis

1. Data inspection and cleaning.
2. Missing-value treatment and data-type conversion.
3. Outlier detection using IQR and Z-score methods.
4. Descriptive statistics and Pearson correlation.
5. Feature creation for total spending and total purchases.
6. A 95% confidence interval for average customer spending.
7. Linear regression of total purchases against total spending.
8. ANOVA comparison of campaign response rates.
9. Visual analysis of distributions, campaign responses, spending, and customer acquisition.

## Notes

- The source notebook referenced a local Windows path. This script uses a command-line path so it can run on other computers.
- The dataset is not embedded in this submission. Make sure you have permission to use and share the dataset.
- Statistical relationships are exploratory and do not by themselves prove causation.
