# Online Retail Exploratory Data Analysis with Python

## Overview

In this project, we will step into the shoes of entry-level data analysts at an online retail company, helping interpret real-world data to make key business decisions. We will employ a mix of classical statistical methods and machine learning techniques to achieve this.

**Classical Statistical Methods**: We will use traditional statistical techniques, such as the Interquartile Range (IQR), to identify outliers and anomalies in the data. These methods are valuable for their simplicity and interpretability, allowing us to detect deviations from expected patterns based on historical data distributions.

**Machine Learning Techniques**: We will also leverage advanced machine learning algorithms, such as Isolation Forest, to enhance our analysis. Machine learning methods are useful for handling complex datasets and detecting subtle patterns that classical methods might miss. By training models on our data, we can identify outliers and anomalies with greater accuracy and robustness.

Combining these approaches allows us to benefit from the strengths of both statistical and machine learning methods. The classical techniques provide a solid foundation for understanding data distributions and basic anomalies, while machine learning techniques offer advanced capabilities for identifying more nuanced outliers and improving the overall reliability of our data analysis. This integrated approach ensures a comprehensive analysis, driving more informed and strategic business decisions.


## Case Study
We will be working with transactional data from an online retail store. The dataset contains information about customer purchases, including product details, quantities, prices, and timestamps. Our task is to explore and analyze this dataset to gain insights into the store's sales trends, customer behavior, and popular products.

By conducting exploratory data analysis, we will identify patterns, outliers, and correlations in the data, allowing us to make data-driven decisions and recommendations to optimize the store's operations and improve customer satisfaction. Through visualizations and statistical analysis, we will uncover key trends, such as the busiest sales months, best-selling products, and the store's most valuable customers. Ultimately, this project aims to provide actionable insights that can drive strategic business decisions and enhance the store's overall performance in the competitive online retail market.

## Data Cleaning and Preparation
- **Handling Missing Values**: Missing values were identified primarily in the 'Description' and 'CustomerID' columns. To streamline the dataset, unnecessary columns such as 'InvoiceNo', 'Description', and 'CustomerID' were dropped. 
- **Data Adjustment**: The 'Country' column was standardized by replacing 'United Kingdom' with 'UK'. Additionally, 'StockCode' values were standardized to ensure consistency across the dataset.

## Outlier Detection Methods
1. **Interquartile Range (IQR)**:
   - The IQR method was used to identify outliers by calculating the range between the 25th and 75th percentiles for 'Quantity' and 'UnitPrice'. This method establishes upper and lower bounds to detect statistical outliers based on the distribution of the data.

2. **Isolation Forest**:
   - **Training**: An Isolation Forest model was trained on the dataset filtered by the IQR method. This machine learning technique was used to identify anomalies by learning from patterns in the data and detecting outliers with a specified contamination rate.
   - **Application**: The model was applied to label data points as outliers or inliers. Outliers detected by the Isolation Forest were excluded to refine the dataset further.

## Results
- The combination of IQR and Isolation Forest methods improved the dataset by reducing variability and providing a cleaner, more reliable set of data for analysis. This enhanced the accuracy of subsequent insights and decision-making based on the dataset.

---
