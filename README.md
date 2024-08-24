# Titanic Survival Prediction Model
This project is a data science analysis and predictive model for the famous Titanic dataset, aimed at determining the likelihood of survival for passengers based on various features. The model was built using Python, and core libraries like Pandas, NumPy, Seaborn, and Scikit-Learn.

![236793-1600x1200-titanic](https://github.com/user-attachments/assets/04456b29-c9a2-469e-9727-30ef17401262)

# Project Overview
The Titanic tragedy is one of the most infamous shipwrecks in history, and this dataset provides insights into passenger details, including age, gender, passenger class, and more. The aim of this analysis is to predict whether a passenger survived or not based on these features.

# Dataset Description
The dataset used for training the model is the Titanic dataset from Kaggle, which consists of two files:

1. train.csv: Contains the data for training, including the target column ("Survived").
2. test.csv: Contains the data for testing, without the target column.

# Data Processing and Cleaning
The steps involved in data cleaning and preprocessing include:

1. Handling missing data by filling or dropping columns with excessive null values.
2. Handling outliers using statistical techniques.
3. Encoding categorical variables.
4. Scaling numerical features for better model performance.
5. Feature selection by dropping irrelevant columns.

# Insights
Here are some key insights derived from the data:

1. Male Survivors: The percentage of males who died is higher than those who survived.
2. Female Survivors: The percentage of females who survived is higher than those who died. This aligns with the priority to save women first.
3. Child Survivors: Most male children aged 0-4 , 12-14 survived, highlighting the priority given to saving children.
4. Old Men Survivors: Most old Male aged 48-50 survived, highlighting the priority given to saving old men.
5. First-Class Males: Males in Pclass 1 had a higher survival rate, especially those aged between 0-18 , 24-28 , 34-36 , 42-44 , 48-50.
6. Large Families: Females with 4 and 6 children all died due to a lack of enough lifeboats.
7. Large Families: Females with 5 children aged 39-42 all died due to a lack of enough lifeboats.

# Storytelling
The survival rates of different groups tell a story of priority during the disaster:

1. Females First: Women were given priority, reflecting the common practice of "women and children first" in evacuations.
2. Childrenand Old Men: The data reveals a strong emphasis on saving young boys and old men.
3. Social Class Matters: Wealthier males in first-class had better chances, indicating that social class played a significant role in survival.
4. Family Size and Survival: Larger families struggled as lifeboats couldn’t accommodate them all, leading to higher mortality rates among those with many dependents.

# Model Building
The Random Forest Classifier model was chosen for this classification task. After training, the model achieved a good accuracy on the training data.
**Training Accuracy: 0.9814814814814815**

# How to Run the Project
1. Clone this repository.
2. Open the notebook in Jupyter or any compatible environment.
3. Ensure the required libraries are installed.
4. Run the notebook step by step to see the analysis and results.

# Prediction Submission
The model generates predictions on the test set and saves the results in submission.csv for submission on Kaggle.
