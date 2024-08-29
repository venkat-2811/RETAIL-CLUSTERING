# Customer Segmentation using K-Means Clustering

## Project Overview

This project aims to perform customer segmentation using K-Means clustering on a dataset of mall customers. The goal is to identify distinct groups of customers based on their annual income and spending score. This segmentation can help businesses understand customer behavior and tailor marketing strategies accordingly.

## Features

- **Customer Segmentation**: The project segments customers into different clusters based on their spending patterns and income.
- **Elbow Method**: Utilizes the Elbow method to determine the optimal number of clusters.
- **Cluster Analysis**: Provides a summary of each cluster's characteristics, including average age, annual income, and spending score.
- **Visualization**: The clusters are visualized using a scatter plot for easy interpretation of the customer segments.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

### Installation

1. **Clone the Repository**:
   ```bash
   git clone (https://github.com/venkat-2811/SCT_ML_2.git)
   cd customer-segmentation
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

   Ensure that the `requirements.txt` file includes:
   ```
   pandas
   numpy
   matplotlib
   seaborn
   scikit-learn
   ```

3. **Download the Dataset**:
   Ensure that the dataset `Mall_Customers.csv` is placed in the project directory.

## Usage

1. **Load the Dataset**:
   The script reads the dataset from `Mall_Customers.csv`.

2. **Select Features for Clustering**:
   The features selected for clustering are 'Annual Income (k$)' and 'Spending Score (1-100)'.

3. **Standardize the Features**:
   The features are standardized using `StandardScaler` to ensure that they are on the same scale, which is important for clustering.

4. **Determine the Optimal Number of Clusters**:
   The Elbow method is used to determine the optimal number of clusters by plotting the within-cluster sum of squares (WCSS) against the number of clusters.

5. **Apply K-Means Clustering**:
   K-Means clustering is applied to the standardized features, and customers are segmented into 5 clusters.

6. **Analyze the Clusters**:
   The clusters are analyzed by calculating the mean values of 'Age', 'Annual Income (k$)', and 'Spending Score (1-100)' for each cluster.

7. **Visualize the Clusters**:
   The clusters are visualized using a scatter plot, with different colors representing different clusters.

8. **Run the Script**:
   To execute the script, run:
   ```bash
   python customer_segmentation.py
   ```

## Project Structure

```
customer-segmentation/
│
├── Mall_Customers.csv          # Dataset used for clustering
├── customer_segmentation.py    # Main script for running the project
├── README.md                   # Project documentation
```

## Results

After running the script, you will get:
- A plot showing the optimal number of clusters using the Elbow method.
- A scatter plot visualizing the customer segments.
- A summary table of the average values for age, income, and spending score within each cluster.

## Future Enhancements

- **Add More Features**: Include additional features such as age, gender, or other relevant data to improve clustering.
- **Experiment with Different Clustering Algorithms**: Try using other clustering algorithms like DBSCAN or hierarchical clustering to compare results.
- **Advanced Visualization**: Use 3D plots or interactive visualizations to better understand customer segments.
