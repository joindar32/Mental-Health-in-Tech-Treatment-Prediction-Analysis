# Mental-Health-in-Tech-Treatment-Prediction-Analysis



This project focuses on analyzing a survey dataset related to mental health in the tech industry and predicting the likelihood of seeking treatment for mental health issues. The project is divided into three key components: data preprocessing, analysis, and model training.

## Files

- `TechSurveyPreprocessing.ipynb`: This notebook handles the preprocessing of the raw survey data. The key steps include:
  - **Data Cleaning**: Handling missing values and standardizing specific columns.
  - **Feature Engineering**: Creating new features, such as age groups.
  - **Output**: The cleaned dataset is saved as `cleaned_df.csv`.

- `TechSurveyAnalysis.ipynb`: This notebook focuses on visualizing the data and performing exploratory data analysis. It includes:
  - **Age Group Analysis**: Examines treatment-seeking behavior across different age groups.
  - **Gender Distribution**: Analyzes the gender distribution of the respondents.
  - **Country-wise Analysis**: Visualizes the distribution of respondents from different countries and their treatment-seeking behavior.
  - **Analysis of Significant Factors**: Investigates the impact of factors like family history, work type, and employer attitude on treatment-seeking behavior.
  - **Significant Features Selection**: Uses the Chi-square test to identify features that significantly influence treatment-seeking behavior and saves the filtered dataset as `df_significant.csv`.

- `TechSurveyModels.ipynb`: This notebook focuses on training and optimizing machine learning models on the preprocessed dataset `df_significant.csv`. It includes:
  - **Model Training**: Training models such as Logistic Regression, Random Forest, XGBoost, SVM, Gradient Boosting, and LightGBM.
  - **Hyperparameter Tuning**: Using GridSearchCV and RandomizedSearchCV to optimize models.
  - **Performance Evaluation**: Comparing models based on accuracy, training time, and prediction speed.

## Getting Started

1. **Install the required libraries**: Ensure that you have the following Python libraries installed:
    ```bash
    pip install pandas numpy seaborn scikit-learn matplotlib xgboost lightgbm
    ```

2. **Run the Preprocessing Notebook**: Open `TechSurveyPreprocessing.ipynb`, run the cells, and generate `cleaned_df.csv`.

3. **Run the Analysis Notebook**: Open `TechSurveyAnalysis.ipynb` to visualize the data and extract significant features into `df_significant.csv`.

4. **Train Models**: Use `TechSurveyModels.ipynb` to train the models and evaluate their performance.

## Data

The dataset consists of a survey that collects information about mental health in the tech industry. The preprocessed version is available as `cleaned_df.csv`, and the dataset with significant features is saved as `df_significant.csv`.

