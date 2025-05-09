# Customer Segmentation for Marketing Strategy

## Project Overview
This repository contains the implementation and analysis of customer segmentation techniques for marketing strategy development. It includes both the Python code implementation and an academic paper analyzing the results.

## Objective
The main goal of this project is to use machine learning clustering algorithms to group customers based on their spending behavior and demographics, enabling the development of tailored marketing strategies.

## Dataset
The project uses the Mall Customer Segmentation dataset from Kaggle, which includes customer information such as:
- CustomerID
- Gender
- Age
- Annual Income (in thousands of dollars)
- Spending Score (1-100)

## Techniques Implemented
1. **K-Means Clustering** - Partitioning customers into distinct groups
2. **DBSCAN Clustering** - Density-based clustering to identify non-spherical clusters and outliers
3. **Principal Component Analysis (PCA)** - For dimensionality reduction and visualization

## Repository Structure
- `customer_segmentation.py` - Main Python script implementing the clustering algorithms
- `customer_segmentation_analysis.ipynb` - Jupyter notebook with detailed analysis and visualizations
- `Mall_Customers.csv` - Dataset (will be downloaded automatically if not present)
- `plots/` - Directory containing generated visualizations
- `segmented_customers.csv` - Output file with cluster assignments

## Requirements
To run this code, you'll need the following Python packages:
```
numpy
pandas
matplotlib
seaborn
scikit-learn
kneed
```

You can install all requirements using:
```
pip install -r requirements.txt
```

## Running the Code
You can run the analysis in two ways:

### Python Script
```
python customer_segmentation.py
```
This will execute the full analysis, generate all plots in the `plots/` directory, and output the segmented data.

### Jupyter Notebook
```
jupyter notebook customer_segmentation_analysis.ipynb
```
This allows you to interactively explore the data, visualizations, and analysis alongside the academic explanation.

## Results
The analysis identifies five distinct customer segments using K-Means:

1. **Standard Customers** - Middle-aged customers with average income and moderate spending
2. **Target Customers** - Young to middle-aged customers with high income and high spending
3. **Conservative Customers** - Older customers with high income but low spending
4. **Careless Customers** - Young customers with lower income but higher spending
5. **Cautious Customers** - Mixed age group with low income and low spending

DBSCAN clustering provides an alternative segmentation approach, identifying clusters of varying shapes and highlighting outliers.

## Marketing Recommendations
For each identified segment, specific marketing strategies are recommended:

- **Target Customers**: Premium loyalty programs, exclusive offers, personalized experiences
- **Conservative Customers**: Value-oriented marketing focused on quality and durability
- **Careless Customers**: Flash sales and popular product offers
- **Standard Customers**: Standard discounts, mid-level discounts, and basic loyalty schemes
- **Cautious Customers**: Consider value alternatives and package deals

## Academic Paper
The repository includes a complete academic analysis of the customer segmentation results in APA format, with sections covering:
- Introduction
- Methodology
- Results
- Discussion
- Conclusion

## Reflections
This project has proven to be greatly insightful when it comes to employing unsupervised learning techniques to customer segmentation in retail settings. Throughout its deployment, some of the key ideas were:
### Challenges and Learnings
Use of unsupervised learning models entailed careful tuning and verification of parameters, especially with DBSCAN where epsilon and min_points parameters were critical in outcomes
- Interpretation of clustering result in a business scenario was more difficult than anticipated, and various visualization techniques were required to convey the results adequately
- The choice between DBSCAN and K-Means illustrated the significance of choosing an algorithm depending on certain characteristics of a dataset and business needs
### Limitations
- The comparatively small dataset (200 customers) can potentially restrict generalizability of findings - The current analysis is also based on population and expenditure data, while the newer customer segment can be satisfactorily served by adding some behavioral and psychographic considerations - This static analysis fails to maintain temporal properties of customer behavior

### Future Directions
- Incorporating additional data sources such as purchase history, browsing behavior, and social media interactions could enhance segment characterization
- Implementing more advanced techniques like hierarchical clustering or ensemble methods might reveal more nuanced customer groups
- Developing an automated pipeline for continuous customer segmentation would allow for dynamic marketing strategy adaptation

Overall, this project demonstrates both the power and limitations of data-driven customer segmentation, highlighting the importance of combining algorithmic findings with domain expertise for effective marketing strategy development.

## License
MIT

## Author
Joshua Blackburn
