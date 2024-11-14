# Life Expectancy Prediction with Polynomial Regression

This project develops a polynomial regression model to predict life expectancy based on a dataset from the World Health Organization (WHO). The model utilizes various health-related features to estimate the expected lifespan of individuals in different countries.

## Dataset

The dataset used in this project is sourced from Kaggle and can be found at the following link: [here](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who).

### Dataset Description

The dataset contains 2,938 rows and 22 columns, with each row representing a country's life expectancy data for a specific year. The columns include:

- **Country**: Name of the country
- **Year**: Year of the observation
- **Status**: Development status (Developed or Developing)
- **Life expectancy**: Average life expectancy in years
- **Adult Mortality**: Adult mortality rate per 1000 population
- **Infant deaths**: Number of infant deaths per 1000 live births
- **Alcohol**: Alcohol consumption per capita
- **Percentage expenditure**: Health expenditure per capita as a percentage of GDP
- **Hepatitis B**: Hepatitis B immunization coverage
- **Measles**: Measles immunization coverage
- **Polio**: Polio immunization coverage
- **Total expenditure**: Total expenditure on health per capita
- **Diphtheria**: Diphtheria immunization coverage
- **HIV/AIDS**: Deaths due to HIV/AIDS per 100,000 population
- **GDP**: Gross domestic product per capita
- **Population**: Total population
- **Thinness 1-19 years**: Percentage of children under 19 years who are thin
- **Thinness 5-9 years**: Percentage of children aged 5-9 who are thin
- **Income composition of resources**: Proportion of income resources available
- **Schooling**: Average years of schooling

### Dataset Location

- **Data/**: This folder will contain the dataset files downloaded from Kaggle.
- **Notebook/**: This folder will house your Jupyter notebooks. **Currently, we are working within the Notebook directory.**

## Project Structure

The main folders and files in the project are structured as follows:

```plaintext
Life-Expectancy/
├── Data/
│   └── [dataset files will be here]
├── Notebook/
│   └── [your Jupyter notebooks will be here] 
└── README.md
```

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
- **Training Set:** 0.8665
- **Test Set:** 0.8479

## Requirements
To run this project, you'll need the following Python libraries:
- `pandas`
- `scikit-learn`
