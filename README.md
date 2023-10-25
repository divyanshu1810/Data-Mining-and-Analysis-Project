# Market Basket Analysis

This project is a demonstration of Market Basket Analysis using the Apriori algorithm. Market Basket Analysis is a technique used to discover associations between items frequently purchased together. It can be applied to various domains, including retail, e-commerce, and more. In this project, we use the Apriori algorithm to identify frequent item sets and association rules within a grocery shopping dataset.

## Installation

Before running the code, make sure to install the `apyori` library by using the following command:

```bash
pip install apyori
```

## Introduction

The Apriori algorithm is utilized to find frequent item sets and generate association rules. It identifies items that are frequently purchased together, allowing businesses to make data-driven decisions and recommendations based on customer purchasing behavior.

## Libraries Used

This project relies on the following Python libraries:

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations and array handling.
- `matplotlib`: For creating data visualizations.
- `seaborn`: For enhancing data visualization.

## Dataset

The dataset used in this project is named "Groceries_dataset[1].csv." It contains information about grocery shopping transactions, including the date, member number, and item descriptions. To load and analyze the dataset, we perform the following steps:

1. Load the dataset using `pandas`.
2. Set the index of the DataFrame to the 'Date' column.
3. Convert the 'Date' column to the datetime format.

### Data Overview

We examine the dataset by performing the following:

- Displaying the shape of the dataset.
- Describing the dataset to gain insights into numerical data.
- Checking for missing values (there are no missing values).

## Data Analysis

We provide an overview of the dataset by calculating and displaying statistics such as the total number of items sold, the number of days the data spans, and the number of months covered.

We also present a bar plot showing the top 20 items purchased by customers.

## Market Basket Analysis

Market Basket Analysis is performed using the Apriori algorithm. The dataset is grouped to create a list of products bought by the same customer on the same date. The Apriori algorithm requires the input data to be in the form of lists, so we convert the dataset accordingly.

The Apriori algorithm is applied with the following parameters:

- `min_support`: Minimum support threshold (0.00030)
- `min_confidence`: Minimum confidence threshold (0.05)
- `min_lift`: Minimum lift threshold (2)
- `min_length`: Minimum length of an itemset (2)

The results of the Apriori analysis are then presented, including the left-hand side, right-hand side, support, confidence, and lift of the generated association rules.

## Conclusion

Market Basket Analysis provides valuable insights into customer behavior and product associations, allowing businesses to make informed decisions regarding product placement, marketing, and recommendations. This project serves as an example of how to perform Market Basket Analysis using the Apriori algorithm in Python.
