# Experiment 10 — Business Intelligence Application using Data Mining

**Data Mining and Business Intelligence (DMBI)** · Class D15A · Group practical

| Field | Detail |
|:--|:--|
| Tool | Python (K-Means, Random Forest), Streamlit and React dashboard |
| Case study | IPL player-role clustering and auction price valuation |
| Report | [`docs/Experiment_10_Report.pdf`](docs/Experiment_10_Report.pdf) *(to be added)* |
| Write-up | [`docs/Experiment_10_Writeup.docx`](docs/Experiment_10_Writeup.docx) |
| Code | Not yet included |
| Data | Not yet included (IPL `deliveries.csv` and `matches.csv`, Kaggle "IPL Complete Dataset", plus the auction list) |

## Summary
Clusters IPL batters and bowlers into role archetypes with K-Means, predicts a fair auction price with a Random Forest validated by leave-one-group-out cross-validation, flags over- and under-valued players by their valuation gap, and presents the results in a dashboard with a bid-ceiling recommendation.

## Outstanding
- `code/`: the Python pipeline and dashboard source (`app.py` and the React app are described in the write-up but were not in the upload).
- `data/`: the IPL dataset and auction list.
