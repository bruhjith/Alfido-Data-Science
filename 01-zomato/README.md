# Task 1 | Zomato restaurant listings

[Executed notebook](analysis.ipynb) · [Executive summary and five recommendations](report.pdf) · [Cleaned outlet table](cleaned_outlets.csv)

The assigned CSV has 56,252 rows. Checking the online-order and table-booking fields identifies 51,717 rows that match the listing schema. Repeated entries occur under several listing categories. The notebook groups them by normalized restaurant name and address and selects the observation with the most votes. This leaves 12,494 outlets, including 3,016 without a usable rating.

Whitefield has the most distinct outlets (886). North Indian is the most common cuisine label (5,033 outlets). Among 9,439 outlets with a price and a rating, the rank correlation is 0.28. All prices are INR for two people. Review text is inconsistent in this extract, so the word cloud uses cuisine labels.

The cleaned table contains an outlet identifier, name, locality, cuisine labels, rating, votes and approximate cost for two. Blank fields represent unavailable values. The notebook regenerates the same table. To run offline, save the original archive as `data/zomato.zip` beside the notebook. [Kaggle source](https://www.kaggle.com/datasets/bhanupratapbiswas/zomato)
