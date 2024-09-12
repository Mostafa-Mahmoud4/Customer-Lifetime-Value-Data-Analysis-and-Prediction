# Customer Lifetime Value (CLV) - Data Analysis and Prediction

This project focuses on analyzing customer purchasing behavior and predicting their **Customer Lifetime Value (CLV)** using historical sales data. The goal is to identify key features such as purchase frequency, recency, and average monetary value to forecast future customer value.

## Dataset

The dataset used in this project is the [Online Retail dataset](https://raw.githubusercontent.com/rajeevratan84/datascienceforbusiness/master/OnlineRetail.xlsx).

The dataset contains transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based online retailer.

## Project Highlights

- **Data Preprocessing**:
  - Removed negative quantities (indicating returns).
  - Filtered out transactions with missing customer IDs.
  - Focused on transactions before December 1, 2011.

- **Feature Engineering**:
  - Created a new `Sales` column to represent the total revenue per transaction.
  - Grouped data by customer and invoice number to generate summary statistics like total sales, average sales, and purchase frequency.

- **Exploratory Data Analysis (EDA)**:
  - Visualized customer purchase patterns.
  - Explored the distribution of time between purchases and purchase frequency.
  
- **Customer Segmentation**:
  - Segmented customers based on their purchase behavior.
  - Grouped customers by sales frequency and average spend per sale.

- **RFM Model**:
  - Defined key metrics for Recency (R), Frequency (F), and Monetary Value (M) to quantify customer value.

- **Predictive Modeling**:
  - Predicted 3-month Customer Lifetime Value (CLV) using **Linear Regression**.
  - Created features for past customer behavior to predict future CLV.
  - Evaluated model performance using R-squared and Median Absolute Error (MAE) on training and test datasets.

## Key Results

- **RFM Analysis**:
  - **R(ecency)**: How recently a customer made a purchase.
  - **F(requency)**: How often a customer made purchases.
  - **M(onetary Value)**: Average spend per transaction.

- **Predictive Model Performance**:
  - In-Sample R-Squared: ~0.5
  - Out-of-Sample R-Squared: ~0.47
  - Median Absolute Error: ~200 for training and test datasets.

- **Key Features for CLV Prediction**:
  - Sales Sum
  - Sales Count
  - Sales Average

## How to Run

1. Clone the repository.
2. Install required packages:
   
     pip install pandas matplotlib scikit-learn
  
3. Download the dataset and run the notebook to perform the analysis and predictions.

## Visualizations

- Bar charts showing customer purchase counts and average sales.
- Histograms illustrating the distribution of time between purchases.
- Scatter plot comparing actual vs. predicted CLV values.

## Conclusion

This analysis provides a comprehensive look into customer purchasing behavior, allowing for better decision-making regarding customer retention and targeting. By predicting Customer Lifetime Value, businesses can focus on high-value customers and optimize their marketing strategies.
