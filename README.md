# sephora-product-analytics
Exploratory product analytics using Python and pandas to analyse product performance, pricing and consumer engagement.
# Sephora Product Performance Analysis

## About the Project

I created this project to practise using Python and pandas on a real dataset outside of my university coursework. I chose Sephora product data because I was interested in looking at a consumer-based dataset and seeing what factors might be related to how well different products perform.

The dataset contains 8,494 Sephora products. I mainly looked at product ratings, price, reviews and loves, as well as differences between brands and product categories.

## What I Looked At

Some of the main questions I explored were:

- Are higher-rated products also more popular?
- Does price have any relationship with ratings or engagement?
- What is the relationship between the number of reviews and loves?
- Which product categories tend to receive the most engagement?
- Which brands have the highest typical engagement?
- What are the most-loved individual products in the dataset?

## Tools

- Python
- pandas
- Matplotlib
- Jupyter Notebook

## Main Findings

- The median product rating was around **4.29**, so ratings were generally quite high across the dataset.
- Loves varied a lot more between products, with a relatively small number of products receiving extremely high engagement.
- There was almost no linear relationship between product rating and loves (**r = 0.042**).
- Price also had very little linear relationship with either ratings or loves.
- Reviews and loves had a much stronger positive relationship (**r = 0.684**).
- Among the larger product categories, **Makeup had the highest median number of loves**.
- **8 out of the 10 most-loved products were Makeup products**.
- For brands with at least 30 products, **Rare Beauty and The Ordinary** had some of the highest median engagement.

## Data Cleaning

Before starting the analysis, I checked the dataset for missing values and duplicates.

There were 278 products with missing ratings and reviews. I excluded these products when analysing ratings or reviews, but kept them for other parts of the analysis where the available data could still be used.

I also checked for duplicate rows and duplicate product IDs and did not find any.

## Limitations

This analysis only uses the products included in this Sephora dataset, so the findings cannot necessarily be applied to the whole beauty market.

Loves and reviews may also be affected by things that are not included in the dataset, such as how long a product has been available, marketing, brand popularity and product availability.

The correlations in this project show relationships between variables, but they do not show that one variable causes another.

## Dataset

The data comes from the **Sephora Products and Skincare Reviews** dataset by **nadyinky** on Kaggle.

## Project File

- `beauty.ipynb` - contains the data cleaning, analysis, visualisations and findings from the project.

The original CSV is not included in this repository and can be downloaded from the Kaggle dataset.

## Running the Notebook

To run the analysis:

1. Download `product_info.csv` from the original Kaggle dataset.
2. Put `product_info.csv` in the same folder as `beauty.ipynb`.
3. Open `beauty.ipynb` using Jupyter Notebook.
4. Run the notebook from top to bottom.
