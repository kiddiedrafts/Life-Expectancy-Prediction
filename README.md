# Life Expectancy Prediction with Polynomial Regression

This project develops a polynomial regression model to predict life expectancy based on a dataset from the World Health Organization (WHO). The model utilizes various health-related features to estimate the expected lifespan of individuals in different countries.

## Dataset
The dataset used for this project is the **Life Expectancy Data** from the WHO, which includes various health indicators such as:
- Adult Mortality
- Child Mortality
- Healthcare Expenditure
- Disease prevalence (e.g., Measles, Diphtheria)
- Socioeconomic factors (e.g., GDP, Education)

The dataset originates from the World Health Organization (WHO) and the United Nations, compiled with contributions from multiple research initiatives.
You can find the dataset [here](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who).


## Feature Engineerin and Data Preprocessing
- Renaming columns to remove extra spaces.
- Handling missing values by dropping rows and filling missing entries with mean or mode values.
- Encoding categorical variables using `LabelEncoder`.
- Dropping unnecessary columns (e.g., 'Country').
- Splitting the dataset into training and testing sets.
- Standard scaling of features for better model performance.
- Generating polynomial features to capture non-linear relationships.

## Model Training
A linear regression model is trained on the polynomial features.
     
## Model Performance
The model achieved the following R² scores:
- **Training Set:** 0.9406
- **Test Set:** 0.9003

## Requirements
To run this project, you'll need the following Python libraries:
- `pandas`
- `scikit-learn`
