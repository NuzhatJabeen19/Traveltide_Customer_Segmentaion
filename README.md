# 🧳 TravelTide Customer Segmentation

A comprehensive data science Academic project focused on analyzing customer behavior for the e-booking platform TravelTide, identifying distinct customer segments, and recommending personalized perks to enhance customer loyalty and retention.

## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Business Objectives](#business-objectives)
- [Project Structure](#project-structure)
- [Dataset Description](#dataset-description)
- [Methodology](#methodology)
- [Key Features](#key-features)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Results & Insights](#results--insights)
- [Technologies Used](#technologies-used)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)

## 🎯 Project Overview

This project analyzes customer behavior patterns in the travel industry using TravelTide's booking platform data. By leveraging advanced analytics and machine learning techniques, we identify distinct customer segments and develop targeted marketing strategies to improve customer retention and business growth.

**Key Deliverables:**
- Customer segmentation analysis
- Personalized perk recommendations for each segment
- Data-driven insights for marketing strategy optimization
- Actionable recommendations for customer retention

## 🚀 Business Objectives

- **Validate Customer Groups:** Identify distinct customer segments receptive to specific perks
- **Personalized Marketing:** Develop targeted perk recommendations for each customer segment
- **Retention Strategy:** Create data-driven approaches to enhance customer loyalty
- **Business Growth:** Inform marketing strategies that drive engagement and revenue

## 📁 Project Structure

The project is organized into three comprehensive Google Colab notebooks:

```
Traveltide_Customer_Segmentation/
│
├── 📓 Notebook 1: Data Retrieval and Cohort Selection
│   ├── Database connection and data extraction
│   ├── Cohort filtering (post-Jan 4, 2023 & 7+ sessions)
│   └── Output: df_cohort.csv
│
├── 📓 Notebook 2: Exploratory Data Analysis (EDA)
│   ├── Comprehensive data exploration
│   ├── User behavior pattern analysis
│   ├── Feature engineering
│   └── Output: user_based_table.csv
│
└── 📓 Notebook 3: Segmentation and Clustering
    ├── Advanced feature engineering
    ├── Rule-based segmentation
    ├── PCA dimensionality reduction
    ├── Clustering algorithms (K-Means, DBSCAN)
    └── Perk recommendations
```

## 📊 Dataset Description

The analysis utilizes TravelTide's comprehensive database including:

- **User Demographics:** Age, location, user preferences
- **Browsing Activity:** Session data, search patterns, engagement metrics
- **Booking Information:** Flight and hotel reservations, pricing, dates
- **Temporal Data:** Booking patterns, seasonality trends

**Cohort Criteria:**
- Records from January 4, 2023 onwards
- Users with more than 7 platform sessions
- Active engagement indicators

## 🔬 Methodology

### 1. Data Preparation
- Database querying and data extraction
- Cohort selection based on business criteria
- Data cleaning and preprocessing

### 2. Exploratory Data Analysis
- Statistical analysis of user behavior
- Visualization of travel patterns
- Identification of key behavioral indicators

### 3. Feature Engineering
- Creation of user-level aggregated features
- Behavioral metric calculations
- Travel preference indicators

### 4. Segmentation Approaches
- **Rule-Based Segmentation:** Business logic-driven grouping
- **Clustering Analysis:** Machine learning-based segmentation
- **Principal Component Analysis:** Dimensionality reduction for clustering

### 5. Validation & Analysis
- Silhouette analysis for cluster quality
- Segment characteristic profiling
- Perk recommendation development

## ✨ Key Features

- **Multi-Modal Segmentation:** Combines rule-based and ML approaches
- **Behavioral Analysis:** Deep dive into customer travel patterns
- **Personalized Recommendations:** Tailored perk suggestions per segment
- **Scalable Framework:** Adaptable methodology for similar platforms
- **Visual Analytics:** Comprehensive data visualization throughout

## 🛠️ Installation & Setup

### Prerequisites
- Google Colab account (recommended)
- Access to TravelTide database (for Notebook 1)

### Required Libraries
```python
# Data Manipulation
import pandas as pd
import numpy as np

# Database Connection
from sqlalchemy import create_engine

# Visualization
import matplotlib.pyplot as plt
import seaborn as sns

# Machine Learning
from sklearn.preprocessing import LabelEncoder, OrdinalEncoder, StandardScaler
from sklearn.decomposition import PCA
from sklearn.cluster import KMeans, DBSCAN
from sklearn.neighbors import NearestNeighbors
from sklearn.metrics import silhouette_score

# Geospatial Analysis
from haversine import haversine
```

## 📖 Usage

### Step 1: Data Retrieval
```python
# Open Notebook 1 in Google Colab
# Connect to TravelTide database
# Run cohort selection queries
# Export df_cohort.csv
```

### Step 2: Exploratory Analysis
```python
# Open Notebook 2 in Google Colab
# Load df_cohort.csv
# Perform comprehensive EDA
# Generate user_based_table.csv
```

### Step 3: Segmentation & Clustering
```python
# Open Notebook 3 in Google Colab
# Load user_based_table.csv
# Apply segmentation techniques
# Generate recommendations
```

## 📈 Results & Insights

### Customer Segments Identified
- **Frequent Business Travelers:** High engagement, premium preferences
- **Leisure Vacation Planners:** Seasonal patterns, price-sensitive
- **Budget-Conscious Explorers:** Cost optimization focus
- **Luxury Experience Seekers:** Premium service preferences

### Sample Recommendations
- **Frequent Flyers:** Discounts on extended hotel stays for short trips
- **Family Travelers:** Package deals and child-friendly accommodations
- **Business Users:** Priority booking and flexible cancellation policies
- **Budget Segment:** Early bird discounts and loyalty point multipliers

### Business Impact
- Enhanced customer retention through personalized experiences
- Improved marketing campaign effectiveness
- Data-driven perk allocation strategy
- Foundation for A/B testing and continuous optimization

## 🔧 Technologies Used

- **Programming:** Python
- **Environment:** Google Colab
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Database:** SQLAlchemy
- **Geospatial:** Haversine library

## 🚀 Future Enhancements

- **Dynamic Segmentation:** Real-time customer segment updates
- **A/B Testing Framework:** Systematic perk effectiveness testing
- **Advanced Analytics:** Chi-squared tests for segment validation
- **Automated Pipeline:** End-to-end automated segmentation process
- **Dashboard Development:** Interactive visualization dashboard
- **Predictive Modeling:** Customer lifetime value prediction

## 🤝 Contributing

Contributions are welcome! Please feel free to:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request
4. Report issues or suggest improvements

## 📝 License

This project is for educational and research purposes. Please ensure proper attribution when using or referencing this work.

## 👤 Author

**Nuzhat Jabeen**
- GitHub: [@NuzhatJabeen19](https://github.com/NuzhatJabeen19)
- LinkedIn: [Connect with me](www.linkedin.com/in/nuzhat-jabeen-amna)

---

⭐ **If you found this project helpful, please give it a star!** ⭐

---

*This project demonstrates the application of data science techniques in the travel industry, showcasing skills in customer analytics, machine learning, and business strategy development.*