# NBA Player Longevity Prediction – Feature Engineering Report

## Target Variable Definition

The `target_5yrs` column was selected as the dependent variable for this project. This variable indicates whether an NBA player remained active in the league for at least five years and serves as the prediction target for future machine learning models.

## Removal of Non-Predictive Features

Non-predictive columns such as player names and identification fields were removed from the dataset. These variables do not contribute meaningful predictive information regarding player longevity and may introduce noise or data leakage into the model.

## Correlation Analysis and Feature Selection

A correlation analysis was performed on the numerical features to identify highly correlated variables. Features exhibiting strong correlations were examined for redundancy, and redundant predictors were considered for removal to reduce multicollinearity and improve model interpretability.

The correlation matrix and heatmap provided insight into relationships among player performance metrics, helping to create a more efficient feature set.

## Feature Engineering

To improve the predictive value of the dataset, a new composite feature was created by combining existing player statistics.

Example:

**Points Per Minute (PPM)**

PPM = Points Scored ÷ Minutes Played

This metric provides a measure of scoring efficiency independent of total playing time and captures player productivity more effectively than raw point totals alone.

Additional engineered metrics may include efficiency ratings or assist-to-turnover ratios depending on the available dataset features.

## Missing Value Handling

The dataset was examined for missing values across all performance-related columns. Missing numerical values were handled using median imputation to preserve observations while minimizing the influence of outliers.

This approach ensured that the dataset remained suitable for machine learning without introducing significant bias.

## Final Dataset Preparation

After feature selection, feature engineering, and missing value treatment, the resulting dataset was cleaned and prepared for predictive modeling. Irrelevant variables were removed, redundancy was reduced through correlation analysis, and meaningful derived metrics were introduced to enhance model performance.

## Conclusion

The feature engineering pipeline successfully prepared the NBA player dataset for machine learning. The target variable was clearly defined, non-predictive features were removed, multicollinearity was addressed through correlation analysis, new performance-based features were engineered, and missing values were handled appropriately. These steps improve model readiness, transparency, and reproducibility for NBA player longevity prediction.
