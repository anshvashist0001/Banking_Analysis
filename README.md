# Bank Marketing Campaign Analysis

An end-to-end exploratory analysis of 45,211 bank marketing records using Python, pandas, NumPy, Matplotlib and Seaborn.

[Open the analysis notebook](Bank_Marketing_Analysis.ipynb)

## Aim

Understand how customer details and campaign history relate to term deposit subscriptions, and identify follow-up ideas that could be tested in a future campaign.

## Main findings

- The overall subscription rate was **11.70%**, with **5,289** subscriptions.
- Records with a successful previous campaign had a **64.73%** subscription rate, but accounted for only **1,511 records**.
- Records with one current-campaign contact had a **14.60%** response rate, compared with **3.93%** for 11 or more contacts. This does not prove that additional calls reduce conversion; unsuccessful contacts may receive more follow-ups.
- **28.8%** of records had an unknown contact channel, which limits channel comparisons.

## Work covered

Data profiling, category and numeric checks, missing-value and sentinel treatment, feature engineering, groupby summaries, DataFrame joins and reshaping, visual EDA, confidence intervals and outlier sensitivity checks. The notebook includes seven chart figures and recommendations tied to the results.

## Run locally

Use Python 3.12. Install the dependencies:

```bash
pip install -r requirements.txt
```

Open `Bank_Marketing_Analysis.ipynb` in Jupyter or VS Code with the Jupyter extension. Select the Python environment where the requirements were installed, then run all cells. Keep the `data` directory next to the notebook and use the repository root as the working directory.

To use JupyterLab, install it separately with `pip install jupyterlab`, then run `jupyter lab`. In Colab, upload the notebook and place `bank-full.csv` in a folder named `data`.

## Files

```text
Bank_Marketing_Analysis.ipynb
requirements.txt
data/
    bank-full.csv
    bank-names.txt
```

The CSV is included, so no download is needed to run the analysis. Optional generated outputs are off by default and excluded from Git.

## Limitations

This is historical observational data from one Portuguese bank. It shows associations, not causal effects or guaranteed improvements. There is no customer ID, complete date, revenue or cost information. Call duration is known only after a call and should not be used for pre-call targeting. No prediction model or measured business improvement is claimed.

## Data source

Moro, S., Rita, P., and Cortez, P. (2014). *Bank Marketing*. [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/222/bank+marketing). [DOI 10.24432/C5K306](https://doi.org/10.24432/C5K306). Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Retrieved 6 October 2026.

Original study for this dataset version: Moro, S., Laureano, R., and Cortez, P. (2011). *Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology*, ESM 2011, pp. 117–121. The original data dictionary and citation are in `data/bank-names.txt`.

The original CSV is unchanged; cleaning and derived columns are described in the notebook.
