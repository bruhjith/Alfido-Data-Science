# Alfido Tech | Data Science Internship

Three projects using the Kaggle datasets assigned in the [Alfido Tech Data Science brief](https://www.alfidotech.com/task/data_science.html). Open a notebook on GitHub to read the code, tables and charts. Each PDF is a one-page executive summary.

| Task | Notebook | Report |
| --- | --- | --- |
| 1. Bengaluru restaurant listings | [Zomato analysis](01-zomato/analysis.ipynb) | [Restaurant discovery recommendations](01-zomato/report.pdf) |
| 2. Historical loan approval prediction | [Model comparison](02-loan-approval/analysis.ipynb) | [Review queue and threshold](02-loan-approval/report.pdf) |
| 3. Instagram engagement | [Content analysis](03-instagram/analysis.ipynb) | [Four-week posting plan](03-instagram/strategy.pdf) |

## Reproduce the analysis

The saved notebooks include executed outputs. For a fresh run, use Python 3.12, open a terminal in this folder and run the following commands.

```shell
python -m pip install -r requirements.txt
python -m jupyterlab
```

Open a task's `analysis.ipynb` and choose **Run → Run All Cells**. The first cell that loads data fetches the public Kaggle archive and checks each source table against its recorded SHA-256 fingerprint. No API token is needed for these public downloads. If an automatic download is unavailable, the per-task README explains where to put a manually downloaded ZIP. The Zomato notebook also writes the cleaned outlet table to its working directory.
