# Global Air Pollution Data Analysis

## Overview

Our project aims to enhance the General Air Quality Index (GAQI) by
analyzing vast air quality data from over 170 nations and 300 cities.
Focusing on pollutants like PM2.5, ozone, carbon monoxide, and nitrogen
dioxide, we seek to understand regional air quality disparities.
Leveraging Apache Spark, PySpark, and NoSQL databases, our approach
enables comprehensive data mining and predictive modeling. By
forecasting pollution patterns, we empower environmental policy-making
and public awareness. Through phases including data acquisition,
preprocessing, analysis, and modeling, our five-week project ensures
accurate GAQI insights. Ultimately, we strive to aid global efforts in
mitigating air pollution\'s adverse effects, promoting a healthier
future.

## DATASET USED:

For this project, we utilize the [Global Air Pollution
dataset](https://www.kaggle.com/datasets/sazidthe1/global-air-pollution-data/data)
available on Kaggle

## Installation and Setup

1. Clone the repository:

bash

git clone \<repository_url\>

cd \<repository_name\>

2. Install dependencies:

bash

pip install -r requirements.txt

3. Databricks Setup:

\- This project can be run on Databricks.

\- Ensure Databricks filesystem (DBFS) is accessible.

\- Create a Databricks cluster to execute the code.

\- Upload the repository to Databricks and access it from the cluster.

4\. Running on Databricks:

\- Create a Databricks cluster with appropriate configurations.

\- Upload the repository to Databricks.

\- Access the notebook or script containing the provided code snippets.

\- Execute the code in the Databricks environment.

## Code Structure

\- global_air_pollution_analysis.ipynb: Main Python script
containing the code for data analysis, preprocessing, model training,
and evaluation.

## Code Overview

1\. Data Loading:

\- The script loads the global air pollution data from the file
global_air_pollution_data.csv into a Pandas DataFrame.

\- DBFS is utilized for accessing files (dbfs:/FileStore).

2\. Data Preprocessing:

\- Various data preprocessing steps are performed, including handling
missing values, renaming columns, converting data types, and creating
new features such as the Global Air Quality Index (GAQI) and GAQI
category.

3\. Exploratory Data Analysis (EDA):

\- EDA is conducted using visualizations such as heatmaps and boxplots
to understand the relationships between variables, identify trends,
distributions, and potential outliers. - Geospatial analysis is
conducted to visualize air quality across different regions using
GeoPandas. The distribution of AQI values by category is plotted on a
world map. Additional analysis includes plotting distributions of AQI
values, counting occurrences of AQI categories, and determining average
AQI values by country and continent.

4\. Feature Selection:

\- Feature selection techniques like variance thresholding and
identifying quasi-constant features are applied to remove irrelevant or
redundant features, improving model efficiency and performance.

5\. Model Training and Evaluation:

\- Several machine learning models including Linear Regression, Decision
Trees, Random Forest are trained and evaluated for predicting GAQI
categories. Model performance metrics such as Mean Absolute Error (MAE),
Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Accuracy
are calculated to assess model efficacy.

## References

\- \[Pandas Documentation\](https://pandas.pydata.org/docs/)

\- \[NumPy Documentation\](https://numpy.org/doc/)

\- \[Matplotlib Documentation\](https://matplotlib.org/contents.html)

\- \[Seaborn Documentation\](https://seaborn.pydata.org/tutorial.html)

\- \[Scikit-learn
Documentation\](https://scikit-learn.org/stable/user_guide.html)

\- \[XGBoost Documentation\](https://xgboost.readthedocs.io/en/latest/)

\- \[PyCountry-Convert
Documentation\](https://pypi.org/project/pycountry-convert/)

\- \[GeoPandas Documentation\](https://geopandas.org/)

\- \[Altair Documentation\](https://altair-viz.github.io/)
