# Kmeans-countries

## Project overview
This project implements a K-means clustering algorithm to group countries based on socio-economic and health factors. The data includes attributes like child mortality, exports, health spending, income, and GDP per capita. The workflow involves data preprocessing, clustering, and performance evaluation using silhouette scores, with visualisations provided for better insights.

## Technologies Used
1) Python
2) Pandas
3) NumPy
4) Scikit-Learn
5) Matplotlib
6) Seaborn

## Dataset
The dataset used for this project is 'country_data.csv', containing various socio-economic and health-related attributes for different countries.

## Project Structure
```markdown
Kmeans_countries/
│
├── data/
│   └── country_data.csv
│
├── notebook/
│   └── Kmeans_countries.ipynb
│
├── results/
│   └── correlation_matrix_of_features.png
│   └── elbow_method.png
│   └── silhouette_score_method.png
│   └── child_mortality_rate_vs_gdp_percapita.png
│   └── inflation_vs_gdp_percapita.png
│
└── requirements.txt
```

## Methodology
1) Data Collection:
   
The project uses the 'country_data.csv' dataset, which was orginally sourced from Help.NGO. This international non-governmental organisation specialises in emergency response, preparedness, and risk mitigation. It includes various socio-economic and health-related attributes for different countries. The key features in the dataset are child mortality, exports, health spending, income, and GDP per capita.

2) Data Preprcessing:
   1. Loading the Data: The dataset is loaded using Pandas, a data manipulation library in Python.
   2. Handling Missing Values: Missing values are not present in this dataset.
   3. Feature Scaling: Features are scaled using normalisation to ensure uniformity and improve the performance of the K-means clustering algorithm.

3) Explanatory Data Analysis (EDA):
   1. Statistical Analysis: Descriptive statistics are computed to understand the distribution and basic statistics of the data.
   2. Data Visualisation: Visual tools such as correlation matrices and scatter plots are used to identify patterns, correlations, and insights within the dataset.

4) Clustering:
   1. Elbow Method: The Elbow method is applied to determine the optimal number of clusters (k) by plotting the within-cluster sum of squares (WCSS) against the number of clusters. This is visualised in elbow_method.png.
   2. Silhouette Score: The silhouette score method is used to evaluate the quality of the clusters and determine the optimal number of clusters. This is visualised in silhouette_score_method.png.
   3. K-means Clustering: The K-means algorithm is implemented to cluster the countries based on the selected socio-economic and health features.

5) Model Evaluation:
   1. Silhouette Score: The silhouette score is calculated to assess the quality and cohesion of the clusters. 
   2. Cluster Visualisation: Clusters are visualised to interpret the results.

## Setup and Installation
1) Clone the repository:
   ```bash
   git clone https://github.com/ellahu1003/country-clustering.git
   cd country-clustering
   ```
2) Install the required packages:
    ```bash
    pip install -r Requirements.txt
    ```
3) Run the Jupyter Notebook:
   ```bash
   jupyter notebook notebooks/Kmeans_countries.ipynb
   ```

## Requirements
The 'Requirements.txt' file lists all the Python packages required to run the project. Install these dependencies to avoid any compatibility issues.

## Results
1) optimum k = 2
2) Silhouette Score: [0.39]
3) The features and their relationships are visualised using a heatmap in correlation_matrix_of_features.png.
4) Determining the optimal number of k using the elbow method is visualised in elbow_method.png.
5) Determining the optimal number of k using the silhouette score method is visualised in silhouette_score_method.png.
6) The clusters for child mortality vs GDPP are visualised in child_mortality_rate_vs_gdp_percapita.png.
7) The clusters for inflation vs GDPP are visualised in inflation_vs_gdp_percapita.png

## Conclusion
1) Child Mortality Rate vs. GDP Per Capita:
   1. Developed countries (Cluster 1) have low child mortality rates and high GDP per capita.
   2. Developing or underdeveloped countries have high child mortality rates and low GDP per capita.
   3. The highest GDP per capita countries in Cluster 1 have almost zero child mortality.
2) Inflation vs. GDP per Capita:
   1. Developed countries (Cluster 1) have higher GDP per capita and lower inflation rates.
   2. Developing and underdeveloped countries (Cluster 2) have lower GDP per capita and higher inflation.
   3. Stable economies with effective policies are represented in Cluster 1.



