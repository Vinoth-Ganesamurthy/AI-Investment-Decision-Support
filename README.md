# AI-Investment-Decision-Support
## Machine Learning Baseline

### Models Tested

The following machine learning algorithms were evaluated for predicting the next day's stock price movement:

- Logistic Regression
- Decision Tree
- Random Forest

### Validation Strategy

To evaluate model performance, **TimeSeriesSplit** cross-validation was used. Unlike a random train-test split, TimeSeriesSplit preserves the chronological order of stock market data, ensuring that the model is always trained on past data and tested on future data. This approach is more appropriate for financial time-series prediction.

### Model Performance

| Model | Average Accuracy |
|--------|-----------------:|
| Random Forest | 49.68% |
| Logistic Regression | 49.63% |
| Decision Tree | 49.26% |

### Key Findings

- Random Forest achieved the highest average accuracy (49.68%).
- Logistic Regression produced nearly identical performance.
- Decision Tree performed slightly worse than the other models.
- The small differences between the models indicate that increasing model complexity alone does not significantly improve prediction accuracy.
- Future improvements should focus on feature engineering by incorporating additional technical indicators and market-related information.