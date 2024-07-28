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
The dataset used for this project is country_data.csv, containing various socio-economic and health-related attributes for different countries.

## Setuo and installation
1) Clone the repository:
   ```bash
   git clone https://github.com/yourusername/country-clustering.git
   cd country-clustering
   ```
2) Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
3) Run the Jupyter Notebook:
   ```bash
   jupyter notebook notebooks/Kmeans_countries.ipynb
   ```

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
│   └── clusters_visualization.png
│   └──
│   └──
│   └──
│   └──
│
└── requirements.txt
```

## Requirements
The requirements.txt file lists all the Python packages required to run the project. Install these dependencies to avoid any compatibility issues.

## Results
1) Silhouette Score: [Insert Silhouette Score here]
2) The clusters and their relationships are visualised in clusters_visualisation.png.

## Conclusion
1) Child Mortality Rate vs. GDP Per Capita:
   1. Developed countries (Cluster 1) have low child mortality rates and high GDP per capita.
   2. Developing or underdeveloped countries have high child mortality rates and low GDP per capita.
   3. The highest GDP per capita countries in Cluster 1 have almost zero child mortality.
2) Inflation vs. GDP per Capita:
   1. Developed countries (Cluster 1) have higher GDP per capita and lower inflation rates.
   2. Developing and underdeveloped countries (Cluster 2) have lower GDP per capita and higher inflation.
   3. Stable economies with effective policies are represented in Cluster 1.



