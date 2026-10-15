# House Prices Prediction: My First Linear Regression Model

My first end-to-end machine learning project, using the Kaggle House Prices dataset to predict residential sale prices.

I built this notebook while teaching myself the fundamentals of machine learning during my PhD, after completing Andrew Ng's Machine Learning and Deep Learning courses on Coursera. The aim was to move beyond theory and work through a real prediction problem, from exploratory data analysis to a Kaggle submission.

## Kaggle result

**Best Score: 18127.17217 (Version 16)**

This was an **approximately average result** on the leaderboard, rather than a top-performing submission. For a first regression project, the main value was learning how to construct, evaluate, and compare models.

[View the Kaggle notebook and submission (V16)](https://www.kaggle.com/code/alexdavidson1995/house-prices-first-linear-regression-model?scriptVersionId=224838656)

## What I did

1. **Exploratory data analysis:** Inspected the data, visualised the distribution of sale prices, plotted individual features against `SalePrice`, and examined correlations and categorical feature distributions.
2. **Preprocessing:** Created a training and validation split, converted categorical variables using one-hot encoding, investigated missing values, and applied median imputation to numerical features.
3. **Feature scaling:** Experimented with MinMax scaling and standardisation.
4. **Regression models:** Trained and compared ordinary linear regression, Ridge regression (L2 regularisation), and Lasso regression (L1 regularisation).
5. **Feature selection:** Tested models using a smaller set of selected features.
6. **Gradient descent:** Implemented gradient descent as a practical exercise to understand parameter optimisation.
7. **Evaluation:** Compared validation results using R² and mean squared error (MSE).
8. **Submission:** Generated predictions for the unseen Kaggle test data using a Ridge regression model and exported them to `submission.csv`.

## Tools

- Python
- pandas and NumPy
- scikit-learn
- Matplotlib and Seaborn
- Jupyter Notebook / Kaggle

## Running the notebook

Open [`house-prices-first-linear-regression-model-final.ipynb`](house-prices-first-linear-regression-model-final.ipynb) in Kaggle or Jupyter.

The notebook currently uses Kaggle dataset paths under:

```text
/kaggle/input/home-data-for-ml-course/
```

To run it locally, download the corresponding training, test and sample submission CSV files, update the input paths, and install the Python libraries listed above. The notebook is an exploratory learning exercise rather than a packaged, reproducible machine learning pipeline.

## What I learned

- Why understanding missing data and feature distributions matters before fitting a model.
- How one-hot encoding allows linear models to use categorical variables.
- How feature scaling and regularisation affect regression workflows.
- Why a separate validation set is important when comparing models.
- How to compare models using more than one metric.
- How gradient descent relates to fitting model parameters.
- How to transform unseen test data consistently before generating predictions.

## Reflections and next steps

This is a record of my first attempt, including the experimentation and imperfections involved in learning. A useful next step would be to consolidate preprocessing and modelling into a `scikit-learn` pipeline, fit transformations only on training folds, and use cross-validation to tune hyperparameters and reduce the risk of data leakage.

## References

- [My Kaggle notebook, Version 16](https://www.kaggle.com/code/alexdavidson1995/house-prices-first-linear-regression-model?scriptVersionId=224838656)
- [House Price Prediction: Linear and Nonlinear Models](https://www.kaggle.com/code/arezoodahesh/house-price-prediction-linear-nonlinear-models), a notebook I found helpful for checking my exploratory analysis.
