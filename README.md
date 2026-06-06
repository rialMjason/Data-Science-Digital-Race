# Data-Science-Digital-Race

**Project**: Analysis and modeling experiments from two team notebooks focused on airline review sentiment analysis and bank customer churn prediction.

**Notebooks**
- [DSDR_round_3.ipynb](DSDR_round_3.ipynb): Exploratory analysis of an airline review dataset. Computes VADER sentiment scores for reviews, generates a scatter plot of `Overall_Rating` vs `sentiment_score`, identifies "inconsistent" reviews (large differences between scaled sentiment and rating), and inspects their characteristics.
- [DSDR_R2_JASON_CHOONG_JIN_SHEN.ipynb](DSDR_R2_JASON_CHOONG_JIN_SHEN.ipynb): Bank customer churn analysis and modeling. Loads `Bank Customer Churn Prediction.csv`, computes churn rate and group statistics, preprocesses features (scaling and encoding), trains models (Logistic Regression, Random Forest, Gradient Boosting), and compares performance metrics.

**Key Findings**
- `DSDR_round_3.ipynb`: A scatter plot visualises rating vs sentiment; with a chosen threshold the notebook identifies many "inconsistent" reviews (example counts reported in the notebook). Negative reviews dominate the inconsistent set, suggesting polarity/rating mismatch in many samples.
- `DSDR_R2_JASON_CHOONG_JIN_SHEN.ipynb`: Models were trained and evaluated; Gradient Boosting showed the strongest overall performance in the notebook's reported metrics, while Random Forest achieved the highest precision.

**Files Used**
- Airline Review.csv
- Bank Customer Churn Prediction.csv

**How to run**
1. Install dependencies (recommended in a virtual environment):

```bash
python -m pip install -r requirements.txt
```

If `requirements.txt` is not present, install these common packages:

```bash
python -m pip install pandas numpy scikit-learn matplotlib seaborn nltk jupyter
```

2. Start Jupyter and open the notebooks:

```bash
jupyter notebook
```

3. For `DSDR_round_3.ipynb`, run the cells in order to compute sentiment scores (VADER will be downloaded if necessary) and produce the scatter plot and inconsistency analysis.
4. For `DSDR_R2_JASON_CHOONG_JIN_SHEN.ipynb`, run the preprocessing and model-training cells. Ensure `Bank Customer Churn Prediction.csv` is available in the working directory.

