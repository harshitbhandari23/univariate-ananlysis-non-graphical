# univariate-ananlysis-non-graphical
🏨 NYC Airbnb Data Analysis (2019)

This project explores the New York City Airbnb Open Data (2019) dataset using Pandas, NumPy, and Seaborn.
It covers data cleaning, categorical analysis, numerical analysis, and basic statistics to understand Airbnb listings distribution across neighborhoods, room types, and pricing.

📌 Project Overview

Cleaned and preprocessed the dataset (removed null values, converted datatypes).

Explored categorical features such as neighbourhood groups, room types, and hosts.

Analyzed numerical features like price distribution, mean, standard deviation, skewness, and kurtosis.

Generated summary statistics and correlations for deeper insights.

📂 Dataset

Source: Airbnb NYC 2019 dataset

File Used: AB_NYC_2019.csv

Contains information about Airbnb listings in NYC:

id, host_id, neighbourhood_group, neighbourhood, room_type

price, minimum_nights, number_of_reviews, latitude, longitude

🔧 Requirements

Make sure you have the following libraries installed:

pip install pandas numpy seaborn matplotlib

🚀 Usage

Run the Python script in Jupyter Notebook or any IDE:

import pandas as pd
import numpy as np
import seaborn as snp

# Load dataset
df = pd.read_csv("AB_NYC_2019.csv")

# Drop missing values
df.dropna(inplace=True)

# Data summary
print(df.info())
print(df.describe())

📊 Analysis Performed
🔹 Categorical Analysis

Distribution of neighbourhood groups

Distribution of room types

Neighbourhoods with more than 1000 listings

🔹 Numerical Analysis

Price distribution using value_counts(bins=5)

Mean, Standard Deviation, Skewness, Kurtosis of price

Correlation matrix (df.corr())

📈 Sample Insights

Certain neighborhoods dominate Airbnb listings (e.g., Manhattan, Brooklyn).

Entire homes/apartments are the most common room type.

Price distribution is highly skewed, indicating a few extremely expensive listings.

📌 Next Steps

Visualize categorical and numerical insights using Seaborn & Matplotlib.

Build predictive models for price estimation.

Explore geospatial visualization using latitude and longitude.

🤝 Contributing

Feel free to fork this repo, improve the analysis, or add visualizations. Pull requests are welcome!

📜 License

This project is licensed under the MIT License.
