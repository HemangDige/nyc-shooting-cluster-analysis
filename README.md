# NYC Shooting Cluster Analysis

## Project Overview
This project analyzes historical shooting incidents in New York City using unsupervised machine learning techniques. The goal is to identify crime patterns, shooting hotspots, and incident clusters based on time, location, and severity.

## Dataset
The dataset contains historical shooting incident records from the New York Police Department (NYPD), including:
Due to dataset size limitations, the dataset is not included in this repository. Please download it from the official NYC Open Data source.

- Date and time of occurrence
- Borough and precinct information
- Latitude and longitude
- Victim demographics
- Perpetrator demographics
- Jurisdiction information
- Fatal and non-fatal shooting indicators

## Objectives
- Perform data cleaning and preprocessing
- Conduct Exploratory Data Analysis (EDA)
- Identify temporal and geographical crime trends
- Apply clustering algorithms to group similar incidents
- Detect shooting hotspots using density-based clustering

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

## Data Preprocessing
- Converted date and time columns into proper formats
- Handled missing demographic values
- Removed records with missing coordinates
- Dropped irrelevant columns
- Standardized numerical features using StandardScaler

## Exploratory Data Analysis
The analysis explored:
- Shootings by hour of day
- Shootings by day of week
- Monthly shooting trends
- Year-wise shooting trends
- Borough-wise distribution
- Precinct-wise distribution
- Fatal vs Non-Fatal incidents
- Victim demographics
- Jurisdiction distribution

## Machine Learning Models

### 1. K-Means Clustering
- Used Elbow Method for cluster selection
- Evaluated using Silhouette Score
- Selected K = 4 clusters

### 2. Agglomerative Hierarchical Clustering
- Ward linkage method
- Compared cluster quality using Silhouette Score

### 3. DBSCAN
- Density-based clustering
- Identified shooting hotspots
- Separated noise and isolated incidents

## Results

### K-Means
- Identified four meaningful incident clusters
- Distinguished incidents based on location and severity

### Agglomerative Clustering
- Produced interpretable crime pattern groups
- Silhouette Score ≈ 0.21

### DBSCAN
- Successfully detected high-risk shooting hotspots
- Identified isolated incidents as noise

## Key Insights
- Shootings occur more frequently during nighttime hours.
- Weekend incidents are relatively higher.
- Summer months show increased shooting activity.
- Brooklyn and Bronx have the highest concentration of incidents.
- Most victims are males aged 18–44 years.
- Most incidents are handled by NYPD Patrol jurisdictions.

## Conclusion
This project demonstrates how clustering techniques can be applied to real-world crime data to identify patterns and high-risk locations. The insights generated can support crime analysis, resource allocation, and public safety planning.

## Future Improvements
- Interactive crime hotspot maps
- Power BI dashboard integration
- Additional geospatial analysis
- Predictive crime trend modeling

## Author
Hemang Dige
