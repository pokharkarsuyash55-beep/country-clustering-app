# 🌍 Global Development Clustering

## 📌 Project Overview

This project aims to segment countries into different development groups using unsupervised machine learning techniques. The clustering is based on various economic, health, environmental, and social indicators such as GDP, life expectancy, infant mortality, internet usage, CO₂ emissions, and health expenditure.

The objective is to identify countries with similar development characteristics and compare different clustering algorithms to determine the most suitable model.

---

## 🎯 Business Objective

The objective of this project is to:

- Analyze global development indicators.
- Group countries with similar development characteristics.
- Compare multiple clustering algorithms.
- Provide meaningful insights for policy-making and economic analysis.
- Deploy the clustering model using Streamlit.

---

## 📂 Dataset

The dataset contains development indicators of countries around the world.

Some important features include:

- Country
- GDP
- Birth Rate
- CO₂ Emissions
- Business Tax
- Ease of Business
- Energy Usage
- Health Expenditure (% GDP)
- Health Expenditure per Capita
- Internet Usage
- Infant Mortality
- Lending Rate
- Life Expectancy
- Population
- Tourism
- Urban Population
- and other socio-economic indicators.

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- Streamlit

---

## 📊 Project Workflow

### 1. Data Loading
- Loaded Excel dataset using Pandas.

### 2. Data Preprocessing
- Checked missing values.
- Filled missing numerical values using Mean.
- Filled categorical values using Mode.
- Removed unnecessary columns.
- Standardized numerical features using StandardScaler.

### 3. Exploratory Data Analysis
- Summary statistics
- Correlation Heatmap
- Distribution plots
- Boxplots
- Outlier detection

### 4. Outlier Handling
- Detected outliers using the IQR method.
- Applied capping (winsorization) to reduce the impact of extreme values.

### 5. Feature Scaling
- Applied StandardScaler before clustering.

### 6. Clustering Algorithms

Implemented:

- K-Means Clustering
- Hierarchical Clustering
- DBSCAN

### 7. Model Evaluation

Models were evaluated using:

- Silhouette Score
- Cluster Distribution
- Visual Analysis

---

## 📈 Results

### K-Means

- Produced well-separated clusters.
- Highest Silhouette Score among all models.
- Selected as the final model.

### Hierarchical Clustering

- Generated meaningful cluster hierarchy.
- Useful for visualization.
- Performance was moderate.

### DBSCAN

- Produced many noise points.
- Created fragmented clusters.
- Low Silhouette Score.
- Not suitable for this high-dimensional dataset.

---

## 🌍 Cluster Interpretation

### Developed Countries

Characteristics:

- High GDP
- High Internet Usage
- High Life Expectancy
- High Health Expenditure
- Low Infant Mortality

---

### Developing Countries

Characteristics:

- Moderate GDP
- Moderate Internet Usage
- Improving Health Indicators
- Growing Economy

---

### Underdeveloped Countries

Characteristics:

- Low GDP
- High Infant Mortality
- Low Life Expectancy
- Low Health Expenditure

---

## 📊 Evaluation Metric

Silhouette Score was used to compare clustering performance.

Higher score indicates better cluster separation.

---

## 🚀 Deployment

The final model was deployed using Streamlit.

Features:

- Upload dataset
- Predict cluster
- View clustered countries
- Interactive visualization

---

## 📁 Project Structure

```
Global-Development-Clustering/
│
├── Dataset/
│   └── World_Development_Dataset.xlsx
│
├── Notebook/
│   └── Global_Development_Clustering.ipynb
│
├── app.py
├── requirements.txt
├── README.md
└── clustered_output.csv
```

---

## 📌 Future Improvements

- PCA for visualization
- Hyperparameter tuning
- Interactive dashboards
- Automatic cluster naming
- Cloud deployment

---

## 👨‍💻 Author

**Suyash Pokharkar**

Data Analyst | Python | SQL | Power BI | Tableau | Machine Learning

---

## ⭐ Key Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Outlier Handling
- Feature Scaling
- K-Means Clustering
- Hierarchical Clustering
- DBSCAN
- Model Evaluation
- Data Visualization
- Streamlit Deployment
