
# README for MSCS_634_Lab_1

## Purpose of the Lab Work

In this lab, I applied data visualization, data preprocessing, and statistical analysis techniques to a breast cancer dataset. The goal was to explore the dataset, clean and preprocess the data, and derive meaningful insights using various data analysis tools and techniques available in Python. By completing this lab, I gained a better understanding of how to:
- Handle missing data
- Detect and remove outliers
- Scale data for better analysis
- Visualize relationships and distributions within the dataset
- Perform statistical analysis to summarize data characteristics

The dataset I used contained 4024 entries with 17 features, including variables such as `Age`, `Tumor Size`, `Estrogen Status`, and `Survival Months`. These features were crucial for understanding breast cancer patient data, and the analysis helped uncover patterns and outliers that can guide further research or clinical decision-making.

## Key Insights from Visualizations and Statistical Measures

From the visualizations and statistical measures I performed, the following insights emerged:

1. **Scatter Plot (Age vs. Tumor Size)**:
   - The scatter plot showed a positive correlation between age and tumor size, indicating that older patients tended to have larger tumors. However, the relationship was not perfectly linear, suggesting that other factors might influence tumor size.

2. **Bar Chart (Marital Status Distribution)**:
   - The bar chart revealed a balanced distribution of marital status categories, showing no bias towards any particular marital status group.

3. **Histogram (Tumor Size Distribution)**:
   - The histogram revealed a right-skewed distribution for tumor size, where most tumors were smaller, but there were a few larger tumors, which appeared to be outliers.

4. **Box Plot (Tumor Size by Estrogen Status)**:
   - The box plot showed differences in tumor size between patients with different estrogen statuses. Patients with a positive estrogen status tended to have smaller tumors.

Through statistical analysis, I found that the `Tumor Size` variable had a significant range (from 1 to 140), with a high standard deviation of 21.12. The median tumor size was 25, with a mode of 15. After handling missing values and removing outliers, the dataset exhibited reduced variability.

## Challenges Faced

One of the challenges I encountered during this lab was managing missing values and outliers. Although the dataset did not initially contain missing values, handling the outliers was more complex. The `Tumor Size` variable had extreme values, such as 140, which I removed using the Interquartile Range (IQR) method to maintain the integrity of the analysis.

Additionally, I scaled the data using Min-Max scaling to normalize the values, making it easier to compare and analyze. This step was important for ensuring that numerical features were on the same scale, which is crucial for analysis methods like correlation calculations.

## Files Included

- **Breast_Cancer.csv**: The dataset I used for analysis.
- **MSCS_634_Lab_1.ipynb**: The Jupyter Notebook that contains all the code for data visualization, preprocessing, and analysis.
- **/screenshots**: Folder containing screenshots of visualizations and results from the statistical analysis.
