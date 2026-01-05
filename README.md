Project Overview: Wine Chemical Analysis & Prediction---
This project implements a complete machine learning pipeline to classify wines into three categories based on their chemical composition. Utilizing the standardized Scikit-learn Wine dataset, 
the project demonstrates core data science workflows including exploratory data analysis (EDA), data cleaning, statistical profiling, and classification modeling.

Data Preparation and EDA---
The workflow begins by importing the dataset into a Pandas DataFrame, containing 178 samples and 13 distinct features such as alcohol content, malic acid, magnesium, and color intensity.

Initial exploration includes a missing value assessment using isnull().sum(), which confirms the dataset is clean with zero null values across all chemical markers . Statistical summaries are generated via df.describe() to understand the mean and distribution of attributes like alcohol (mean ~13.00%) and total phenols (mean ~2.30) .

To visualize the relationship between chemical properties, a high-resolution correlation heatmap is generated using Seaborn and Matplotlib . This visualization allows for the identification of
strong multicollinearity between features—for example, the significant positive correlation between flavanoids and total_phenols.

Model Training and Performance-----
The classification phase involves training a machine learning model (using Scikit-learn) to predict the wine "target" class. The dataset is typically split into training and testing sets to validate performance.

The results are evaluated using an accuracy metric. In this specific implementation, the model demonstrates exceptional predictive power, achieving an accuracy score of 100% on the evaluation set.
This indicates that the chemical features provided in the dataset are highly distinct, allowing the classifier to perfectly separate the three wine varieties based on their unique chemical "fingerprints."

Conclusion----
This project serves as a robust example of multi-class classification. It successfully bridges the gap between raw data analysis and high-performance predictive modeling,
making it a valuable addition to any data science portfolio.

--Author: Aditi Tiwari 
--Technologies used: Python, Scikit-learn, Pandas, Seaborn, Matplotlib.
