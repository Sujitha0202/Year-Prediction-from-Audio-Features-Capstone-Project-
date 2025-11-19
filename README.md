#Capstone Project: Year Prediction from Audio Features

##Domain: Entertainment

This project aims to predict the **year of release** for songs using
machine learning models based on audio features.

------------------------------------------------------------------------

## Dataset

-   **Dataset:** YearPredictionMSD\
-   **Source:** UCI Machine Learning Repository\
-   **Rows:** 515,345\
-   **Features:** 90 audio-based attributes\
-   **Target:** Year of release

A 20,000-row sample was used for EDA due to dataset size.

------------------------------------------------------------------------

## Exploratory Data Analysis (EDA)

-   Checked missing values (none found)
-   Summary statistics examined
-   Year distribution visualized
-   Correlation heatmap revealed weak relationship between features and
    year

------------------------------------------------------------------------

## Preprocessing

-   Train-test split: 80/20\
-   StandardScaler used for Linear Regression\
-   Random Forest trained on **unscaled** data (tree models don't
    require scaling)

------------------------------------------------------------------------

## Models Used

1.  **Linear Regression** -- baseline model\
2.  **Random Forest Regressor** -- ensemble model

------------------------------------------------------------------------

## Model Performance

  Model               MSE     MAE    R²
  ------------------- ------- ------ -------
  Linear Regression   94.00   6.83   0.233
  Random Forest       94.77   6.96   0.227

These results are normal because the dataset has weak correlations and
is naturally hard to predict.

------------------------------------------------------------------------

## Feature Importance

Random Forest showed some timbre features influencing predictions, but
overall impact remained weak.

------------------------------------------------------------------------

## Conclusion

This project demonstrates: - A complete ML workflow\
- Understanding of regression models\
- Realistic performance based on dataset nature

Predictions fall within expected ranges (R²: 0.20--0.35 in research).

------------------------------------------------------------------------

## Contents

-   Colab code
-   PPT presentation
-   Report
-   README.md

