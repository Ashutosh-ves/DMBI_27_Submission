# Data Mining and Business Intelligence (DMBI) — Lab Submission

**Student:** Ashutosh Mishra · **Roll No.:** 27 · **Class:** D15A · **Course:** Data Mining and Business Intelligence (DMBI)

All practicals are built on one case study: the **Internship & Project Matchmaking Platform**, which connects students with internship and project openings and tracks their applications. Experiment 10 is a group practical on a separate case study.

## Experiment index

| No. | Experiment | Tool | Code | Data | Status |
|:--:|:--|:--|:--|:--|:--|
| [01](Experiment_01/README.md) | Design of Star and Snowflake Schema | Conceptual data-warehouse design (no code) | — | — | Write-up ready, PDF to add |
| [02](Experiment_02/README.md) | Data Preprocessing Using Python | Python (pandas, scikit-learn) on Google Colab | [`code/Experiment_02.ipynb`](code/Experiment_02.ipynb) | `application_matching_dataset.csv` | Write-up ready, PDF to add |
| [03](Experiment_03/README.md) | Exploratory Data Analysis and Visualization | Python (pandas, matplotlib, seaborn) on Google Colab | [`code/Experiment_03.ipynb`](code/Experiment_03.ipynb) | `application_matching_dataset.csv` | Write-up ready, PDF to add |
| [04](Experiment_04/README.md) | Classification using Decision Tree and Naive Bayes (Weka) | Weka (J48, Naive Bayes, CostSensitiveClassifier) | Weka GUI (no code) | `application_matching_weka.csv` | Write-up ready, PDF to add |
| [05](Experiment_05/README.md) | Classification using Python and User-Defined Functions | Python (scikit-learn) on Google Colab | [`code/Experiment_05.ipynb`](code/Experiment_05.ipynb) | `application_matching_exp5.csv` | Write-up ready, PDF to add |
| [06](Experiment_06/README.md) | K-Means Clustering using Python | Python (scikit-learn) on Google Colab | [`code/Experiment_06.ipynb`](code/Experiment_06.ipynb) | `application_matching_exp67.csv` | Write-up ready, PDF to add |
| [07](Experiment_07/README.md) | K-Means Clustering using Weka | Weka (SimpleKMeans) | Weka GUI (no code) | `application_matching_exp67.csv` | Write-up ready, PDF to add |
| [08](Experiment_08/README.md) | Association Rule Mining (Apriori) using Python | Python (pandas, mlxtend) on Google Colab | [`code/Experiment_08.ipynb`](code/Experiment_08.ipynb) | `skill_profiles_long.csv`, `skill_baskets_weka.csv` | Write-up ready, PDF to add |
| [09](Experiment_09/README.md) | Association Rule Mining (Apriori) using Weka | Weka (Apriori) | Weka GUI (no code) | `skill_baskets_weka.csv` | Write-up ready, PDF to add |
| [10](Experiment_10/README.md) | Business Intelligence Application using Data Mining | Python, Streamlit / React | Not yet included | Not yet included | Write-up ready, PDF to add; code and data outstanding |

## Repository layout

```text
DMBI-Submission/
├── README.md
├── requirements.txt
└── Experiment_01/ … Experiment_10/
    ├── README.md     # aim, tool, files, summary
    ├── code/         # Colab notebooks (.ipynb), Python experiments only
    ├── data/         # datasets used by the experiment
    └── docs/         # write-up (.docx) and lab report (.pdf)
```

## How to run

**Python experiments (2, 3, 5, 6, 8)**: open the notebook in Google Colab, or run it locally.

1. Install the requirements: `pip install -r requirements.txt`
2. Place the matching CSV from `data/` in the same folder as the notebook (or upload it when prompted).
3. Run the cells in order.

Notes:
- Experiments 2 and 8 contain a Colab-only line (upload or download). Skip those lines when running outside Colab.
- Experiment 8 needs `mlxtend`, which is listed in `requirements.txt`.

**Weka experiments (4, 7, 9)**: open the CSV from `data/` in Weka Explorer and follow the steps in the write-up in `docs/`.

**Experiment 1** is a schema design with no code. **Experiment 10** has its write-up; its code and data are still outstanding.

## Dataset summary

| File | Rows | Used in | Description |
|:--|--:|:--|:--|
| `application_matching_dataset.csv` | 673 | 2, 3 | Raw application records with deliberate data-quality issues |
| `application_matching_weka.csv` | 650 | 4 | Cleaned application data for Weka classification |
| `application_matching_exp5.csv` | 650 | 5 | Application data with an engineered `Elite_Match` target |
| `application_matching_exp67.csv` | 300 | 6, 7 | Applicant features with disclosed engineered personas |
| `skill_profiles_long.csv` | 6,214 | 8 | Student skill profiles (long format) |
| `skill_baskets_weka.csv` | 1,318 | 8, 9 | Skill-basket transactions (1,318 × 23) |

Synthetic and engineered data is used where the write-up says so. These datasets are for academic practice, not live platform records.
