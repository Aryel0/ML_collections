# Machine Learning Portfolio - Top Projects

A curated collection of **3 high-impact machine learning projects** demonstrating expertise in data analysis, predictive modeling, and real-world problem-solving using Python and scikit-learn.

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-Latest-orange.svg)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Latest-green.svg)](https://pandas.pydata.org/)

---

## Projects Overview

| Project | Type | Dataset Size | Key Techniques | Impact |
|---------|------|--------------|----------------|--------|
| **Spotify Music Analysis** | Clustering & EDA | 28,680 tracks | K-Means, Genre Analysis | Music Analytics |
| **Apartment Rent Prediction** | Regression | 10,000 listings | Geospatial, Feature Engineering | Real Estate Pricing |
| **Anemia Classification** | Multi-class Classification | 33,924 patients | PCA, Random Forest | Healthcare Diagnosis |

---

## Featured Projects

### 1. Spotify Music Analysis

**Comprehensive Music Analytics & Genre Clustering**

![Project Status](https://img.shields.io/badge/Status-Complete-success)
![Difficulty](https://img.shields.io/badge/Difficulty-Advanced-red)

#### Overview

Analyzes Spotify's audio features to understand music trends, genre characteristics, and what makes songs popular. This project demonstrates advanced exploratory data analysis and unsupervised learning techniques.

#### Objectives

- Identify patterns in music genres using audio features
- Cluster songs based on acoustic characteristics
- Analyze relationships between features and popularity
- Discover trends in modern music

#### Dataset

- **Size**: 28,680 songs
- **Features**: 16 audio attributes
  - Danceability, Energy, Loudness, Speechiness
  - Acousticness, Instrumentalness, Liveness, Valence
  - Tempo, Duration, Key, Mode, Time Signature
- **Source**: Spotify API data with genre labels

#### Techniques Used

- **Exploratory Data Analysis**: Distribution plots, correlation heatmaps
- **Feature Engineering**: Genre encoding, feature scaling
- **Clustering**: K-Means algorithm for genre grouping
- **Visualization**: Seaborn, Matplotlib for insights

#### Key Findings

- **Genre Clusters**: Successfully identified 5-7 distinct music clusters
- **Feature Correlations**: Energy and loudness are highly correlated (r=0.76)
- **Popularity Drivers**: Danceability and energy show positive correlation with popularity
- **Genre Characteristics**: Each genre has unique audio fingerprints

#### Business Value

- **Music Recommendation**: Basis for similarity-based recommendations
- **Playlist Generation**: Automated playlist creation by mood/energy
- **Artist Insights**: Help artists understand genre characteristics
- **Market Analysis**: Identify emerging music trends

#### Files

- `MBINGUI_Ariel_TD7_spotify.ipynb` - Main analysis notebook
- `MBINGUI_Ariel_TD7_spotify.pdf` - Detailed report
- `data_w_genres.csv` - Dataset with genre labels

---

### 2. Apartment Rent Prediction

**Real Estate Price Prediction with Geospatial Analysis**

![Project Status](https://img.shields.io/badge/Status-Complete-success)
![Difficulty](https://img.shields.io/badge/Difficulty-Advanced-red)

#### Overview

Predicts apartment rental prices across multiple U.S. cities using property features, location data, and amenities. This project showcases real-world regression modeling with complex feature engineering.

#### Objectives

- Build accurate rent prediction model
- Identify key factors affecting rental prices
- Analyze geographic price variations
- Provide insights for renters and landlords

#### Dataset

- **Size**: 10,000 apartment listings
- **Features**: 22 attributes including:
  - Location: City, State, Latitude, Longitude
  - Property: Bedrooms, Bathrooms, Square Footage
  - Amenities: Parking, Pets, Utilities
  - Text: Descriptions, Titles
- **Target**: Monthly rent price (USD)

#### Techniques Used

- **Data Preprocessing**: Missing value imputation, outlier detection
- **Feature Engineering**:
  - Geospatial features from lat/long
  - Text feature extraction from descriptions
  - Categorical encoding (One-Hot, Label)
- **Models**: Linear Regression, Random Forest, Gradient Boosting
- **Evaluation**: RMSE, R², MAE, Cross-validation

#### Results

- **Best Model**: Random Forest Regressor
- **Performance**: R² = 0.68, RMSE = $245
- **Key Predictors**:
  1. Location (Latitude/Longitude) - 45% importance
  2. Number of bedrooms - 20% importance
  3. Square footage - 15% importance
  4. City/State - 12% importance

#### Business Value

- **Renters**: Estimate fair market prices, avoid overpaying
- **Landlords**: Competitive pricing strategy
- **Real Estate Agents**: Quick property valuation
- **Market Analysis**: Identify undervalued areas

#### Files

- `MBINGUI_Ariel_TD5_rent.ipynb` - Main analysis notebook
- `apartments_for_rent_classified_10K.csv` - Dataset

---

### 3. Anemia Classification

**Healthcare Diagnosis Using Machine Learning**

![Project Status](https://img.shields.io/badge/Status-Complete-success)
![Difficulty](https://img.shields.io/badge/Difficulty-Intermediate-yellow)

#### Overview

Predicts anemia severity levels in children using demographic and health indicators. This project demonstrates multi-class classification in healthcare with emphasis on recall for medical diagnosis.

#### Objectives

- Classify anemia severity (Not Anemic, Mild, Moderate, Severe)
- Identify key health risk factors
- Support public health interventions
- Prioritize recall over precision for medical safety

#### Dataset

- **Size**: 33,924 patient records
- **Features**: 14 health and demographic attributes
  - Age, Education, Wealth Index
  - Births in last 5 years, Age at first birth
  - Mosquito net usage, Smoking status
  - Marital status, Fever history
  - Hemoglobin level, Iron supplement intake
- **Target**: Anemia level (4 classes)

#### Techniques Used

- **Data Preprocessing**:
  - SimpleImputer for missing values
  - OneHotEncoder for categorical features
  - StandardScaler for normalization
- **Dimensionality Reduction**: PCA (39 → 4 components, 28% variance)
- **Models Compared**:
  - Logistic Regression (Best)
  - K-Nearest Neighbors
  - Support Vector Classifier
  - Decision Tree
  - Random Forest

#### Results

| Model | F1-Score | Precision | Recall |
|-------|----------|-----------|--------|
| **Logistic Regression** | **0.39** | **0.33** | **0.47** |
| K-Nearest Neighbors | 0.37 | 0.37 | 0.37 |
| SVC | 0.38 | 0.33 | 0.46 |
| Decision Tree | 0.35 | 0.37 | 0.34 |
| Random Forest | 0.38 | 0.39 | 0.38 |

**Why Logistic Regression?**

- Highest **recall (0.47)** - critical for medical diagnosis
- Minimizes false negatives (missing anemic patients)
- Better interpretability for healthcare professionals

#### Medical Relevance

- **Early Detection**: Identify at-risk children
- **Resource Allocation**: Target interventions effectively
- **Risk Factors**: Understand anemia predictors
- **Public Health**: Support policy decisions

#### Files

- `MBINGUI_Ariel_TD4_Anemia.ipynb` - Main analysis notebook
- `children_anemia_adjusted.csv` - Dataset

### Machine Learning Algorithms

- **Regression**: Linear, Random Forest, Gradient Boosting
- **Classification**: Logistic Regression, SVM, Decision Trees, KNN
- **Clustering**: K-Means
- **Dimensionality Reduction**: Principal Component Analysis (PCA)

### Data Processing Techniques

- Missing value imputation (SimpleImputer)
- Categorical encoding (OneHot, Label)
- Feature scaling (StandardScaler, MinMaxScaler)
- Train-test splitting & Cross-validation
- Feature engineering & selection

---

## 📈 Skills Demonstrated

### 1. **Data Analysis & Preprocessing**

Handling large datasets (10K-33K samples)  
Missing value treatment strategies  
Outlier detection and handling  
Feature encoding and transformation  

### 2. **Feature Engineering**

Geospatial feature creation  
Text feature extraction  
Dimensionality reduction (PCA)  
Domain-specific feature creation  

### 3. **Machine Learning**

Supervised learning (Regression & Classification)  
Unsupervised learning (Clustering)  
Model selection and comparison  
Hyperparameter tuning  

### 4. **Model Evaluation**

Regression metrics (RMSE, R², MAE)  
Classification metrics (F1, Precision, Recall)  
Business-aligned metric selection  

### 5. **Data Visualization**

Exploratory visualizations  
Correlation analysis  
Distribution plots   

## Getting Started

### Prerequisites

```bash
# Install required packages
pip install pandas numpy scikit-learn matplotlib seaborn plotly
```

1. **Navigate to project folder and run the notebook**

- Spotify Analysis: `MBINGUI_Ariel_TD7_spotify.ipynb`
- Rent Prediction: `MBINGUI_Ariel_TD5_rent.ipynb`
- Anemia Classification: `MBINGUI_Ariel_TD4_Anemia.ipynb`

## Key Insights & Learnings

### Technical Insights

**1. Feature Engineering > Algorithm Selection**

- Well-engineered features often outperform complex models
- Domain knowledge crucial for creating meaningful features
- Geospatial and text features add significant value

**2. Model Interpretability Matters**

- Simpler models preferred in healthcare (Logistic Regression)
- Feature importance helps stakeholder communication
- Trade-off between accuracy and explainability

**3. Metric Selection is Critical**

- Healthcare: Recall > Precision (avoid false negatives)
- Real Estate: RMSE for dollar-value interpretation
- Music: Silhouette score for cluster quality

**4. Data Quality > Data Quantity**

- Clean, relevant features beat large noisy datasets
- Proper preprocessing essential for model performance
- Missing value strategy impacts results significantly

### Domain-Specific Insights

**Music Industry:**

- Genre boundaries are fluid; clustering reveals overlaps
- Danceability and energy drive modern music trends
- Acoustic features predict genre better than metadata

**Real Estate:**

- Location is the strongest price predictor (45% importance)
- Non-linear relationships between features and price
- Text descriptions contain valuable pricing signals

**Healthcare:**

- Class imbalance common in medical datasets
- Multiple weak predictors better than single strong one
- Recall prioritization critical for patient safety


</div>
