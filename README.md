# TravelTide Customer Segmentation and Perk Recommendation Project

This project aims to analyze customer behavior for the e-booking platform TravelTide, identify distinct customer segments, and recommend appealing perks for each segment to enhance customer loyalty and retention. The analysis utilizes data from TravelTide's database, encompassing user demographics, browsing activity, and flight and hotel booking information.

## Project Description

The primary objectives of this project are:

1.  **Validate the existence of customer groups receptive to specific perks.**
2.  **Recommend a potentially appealing perk for each customer segment.**

This data-driven approach is designed to inform a more personalized and effective marketing strategy, ultimately enhancing customer retention and fostering business growth. The project involves data retrieval, exploratory data analysis, feature engineering, and the application of rule-based segmentation and clustering techniques to identify meaningful customer groups.

## Getting Started

This project is structured into three Google Colab notebooks:

1.  **Data Retrieval and Cohort Selection:** This notebook focuses on retrieving data from the TravelTide database, selecting a relevant cohort of users based on specified criteria (records after January 4, 2023, and users with more than 7 sessions), and preparing the data for subsequent analysis. The output of this notebook is a CSV file (`df_cohort.csv`) containing the filtered cohort data.
    -   [Link to Notebook #1](https://drive.google.com/file/d/1oqZ2FsEBxgczXu-DlsxMo1XQIMMgAnP1/view?usp=sharing)

2.  **Exploratory Data Analysis (EDA) and User-Based Table Creation:** This notebook performs extensive exploratory data analysis on the cohort data to understand user behavior and travel patterns. It also involves feature engineering to create relevant features and aggregates session and trip information to create a user-based table (`user_based_table.csv`) suitable for segmentation and clustering.
    -   [Link to Notebook #2](https://colab.research.google.com/drive/1nNKIfJUCpx0ck2U2BAn800pSYgmSdw-T?usp=sharing)

3.  **Feature Engineering, Segmentation, and Clustering:** This notebook implements feature engineering techniques, applies rule-based segmentation, and utilizes Principal Component Analysis (PCA) for dimensionality reduction followed by clustering algorithms (K-Means, DBSCAN) to identify distinct customer segments. Finally, it analyzes the characteristics of each segment to recommend potentially appealing perks.
    -   [Link to Notebook #3](https://colab.research.google.com/drive/1LrMeTDgjzStPT4a8MwGloUZSqwEHLKvr?usp=sharing)

To run these notebooks:

1.  Open the notebook links in Google Colab.
2.  Ensure you have access to the necessary data (the database in Notebook #1 and the generated CSV files in subsequent notebooks).
3.  Run the cells sequentially in each notebook.

## Libraries Used

The following Python libraries are used in this project:

-   `sqlalchemy`
-   `pandas`
-   `numpy`
-   `matplotlib`
-   `seaborn`
-   `scikit-learn` (including `LabelEncoder`, `OrdinalEncoder`, `StandardScaler`, `PCA`, `KMeans`, `DBSCAN`, `NearestNeighbors`, `silhouette_score`)
-   `haversine`

These libraries are commonly available in the Google Colab environment.

## Results

The project successfully identified distinct customer segments within TravelTide's user base through both rule-based and clustering approaches. By analyzing the characteristics and behaviors of these segments (e.g., travel frequency, engagement level, budget preferences, booking habits), potentially appealing perks were recommended for each group. For instance, the report suggests perks like discounts on longer hotel stays for frequent flyers preferring short trips.

The insights gained from this analysis can be used by TravelTide to implement targeted marketing campaigns, personalize customer experiences, and ultimately improve customer retention and loyalty, driving improved engagement and sustained business growth. Further recommendations include dynamic perk allocation, A/B testing, Chi-Squared tests for segment analysis, personalized marketing communications, and continuous updates based on customer feedback.
