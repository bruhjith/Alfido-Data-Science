# Task 2 | Loan approval prediction

[Executed notebook](analysis.ipynb) · [Model comparison and queue recommendation](report.pdf)

The assigned file has 614 applications, including 422 recorded approvals and 192 declines. Credit history is missing in 50 rows. Imputation, scaling, encoding and class weighting are fitted within the training workflow.

The notebook compares logistic regression and a random forest using five-fold predictions on 491 development cases. It selects the model and review threshold before scoring the 123 held-out cases. At the selected 0.47 cutoff, the forest puts 93 files in a priority queue. That includes 78 of the 85 historical approvals. The file contains historical decisions rather than subsequent repayment outcomes.

To run offline, save the original archive as `data/loan-approval-prediction-case-study.zip` beside the notebook. [Kaggle source](https://www.kaggle.com/datasets/bhanupratapbiswas/loan-approval-prediction-case-study)
