# Titanic Survival Prediction Model

This project is a data science analysis and predictive model for the famous Titanic dataset, aimed at determining the likelihood of survival for passengers based on various features. The model was built using Python and core libraries like Pandas, NumPy, Seaborn, and Scikit-Learn.

![236793-1600x1200-titanic](https://github.com/user-attachments/assets/04456b29-c9a2-469e-9727-30ef17401262)

## Project Overview
The Titanic tragedy is one of the most infamous shipwrecks in history, and this dataset provides insights into passenger details, including age, gender, passenger class, and more. The aim of this analysis is to predict whether a passenger survived or not based on these features.

## Dataset Description
The dataset used for training the model is the Titanic dataset from Kaggle, which consists of two files:
- `train.csv`: Contains the data for training, including the target column ("Survived").
- `test.csv`: Used for generating predictions.

## Data Processing and Cleaning
The steps involved in data cleaning and preprocessing include:
1. Handling missing data by filling or dropping columns with excessive null values.
2. Handling outliers using statistical techniques.
3. Encoding categorical variables.
4. Scaling numerical features for better model performance.
5. Feature selection by dropping irrelevant columns.

## Insights
Here are some key insights derived from the data:
1. **Male Survivors**: The percentage of males who died is higher than those who survived.
2. **Female Survivors**: A higher percentage of females survived compared to those who died, reflecting the "women first" rescue priority.
3. **Child Survivors**: Most male children aged 0-4 and 12-14 survived, indicating that young children were prioritized.
4. **Older Men Survivors**: Males aged 48-50 had a higher survival rate.
5. **First-Class Males**: Males in Pclass 1 had a higher survival rate, especially those aged between 0-18, 24-28, 34-36, 42-44, and 48-50.
6. **Large Families**: Females with 4-6 children all perished due to insufficient lifeboats.

## Storytelling
The survival rates tell a compelling story of how priorities during the evacuation were determined by gender, age, and social class:
1. **Females First**: Women were prioritized in rescue efforts.
2. **Children and Old Men**: Young children and older men were given preference for survival.
3. **Social Class Matters**: Wealthier males in first-class had a better chance of survival.
4. **Family Size and Survival**: Larger families struggled, as lifeboats couldn’t accommodate them all.

## Final Predictions
The model was used to make predictions on new test data without the "Survived" column, and the predictions were saved in a Kaggle submission file.

## Model Building
The dataset was split into training and test sets to evaluate model performance. A Decision Tree model was built, and hyperparameters were tuned using `GridSearchCV` with 5-fold cross-validation. The best hyperparameters found were:
- `max_depth`: 10
- `min_samples_leaf`: 2
- `min_samples_split`: 8

After tuning, the model's performance was as follows:
- **Training Score**: 0.8842
- **Test Score**: 0.8208

Learning curves and complexity curves were also plotted to understand the model's behavior and prevent overfitting.
