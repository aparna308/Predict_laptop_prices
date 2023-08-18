Goal- The dataset contains 19 columns describing different features of laptop. Based on the features, model has to predict the laptop price.
Solution Approach- I have done data analysis and data preprocessing, then created a linear regression model. To see how well the model is working, I have calculated the mean square error and varience.
Result- mean_squared_error of the model is 192193347 and varience is 76.6%. Variance evaluates the scatter of the data points around the fitted regression line. 
Higher Variance values represent smaller differences between the observed data and the fitted values.

Detailed Solution-
The dataset has the following features-
1. Brand
2. processor_brand
3. processor_name
4. processor_gnrtn
5. ram_gb
6. ram_type
7. ssd
8. hdd
9. os
10. os_bit
11. graphic_card_gb
12. weight
13. warranty
14. Touchscreen
15. msoffice
16. rating
17. Number of Ratings
18. Number of Reviews
19. Price

The dataset contains 824 entries.
A high level walk through of the steps I followed to make the model-
1. Import all the required libraries and dataset.
2. Checked if dataset has rows with null values, if so then delete them. In this dataset, there were no such rows.
3. Remove dublicate rows.
4. Use seaborn to build graphs visualizing different categories in each column and how many rows belong to each category.
5. There are a lot of "Not Available" present in processor generation column, so I replaced it with most common value of that column.
6. Remove outliers from the 3 numerical columns.
7. Price is dependent column (y), X is all other columns.
8. Create dummy variables for all categorical columns.
9. Split the dataset into train and test set.
10. Create linear regression model.
11. Plot the model's predictions vs actual y values.
12. Calculated the mean_absolute_error and Variance.
