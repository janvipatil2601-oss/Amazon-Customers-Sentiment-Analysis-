# Amazon-Customers-Sentiment-Analysis (Interactive Dashboard using Power BI)

## Project Objective
- Analyze Amazon product review data. 
- Clean and preprocess customer review text. 
- Classify reviews into Positive, Neutral, and Negative sentiments. 
- Compare sentiment across different product categories. 
- Analyze rating distribution and customer feedback. 
- Track review trends over time.

## Dataset
-<a href="https://github.com/janvipatil2601-oss/Amazon-Customers-Sentiment-Analysis-/blob/main/Amazon_Customer_Sentiment_Synthetic_15000.xlsx">Dataset</a>

## Project Process
### Step 1: Data Collection
Collected Amazon customer reviews dataset containing product information, ratings, review titles, review text, verified purchase details, and review dates.
### Step 2: Data Cleaning
- Removed duplicate records.
- Removed missing values.
- Standardized product categories.
- Created Review Length column.
- Created Sentiment column from ratings. 
### Step 3: DAX Measures Created
- Total Reviews
Total Reviews = COUNT('Sheet'[Review_ID])

- Average Rating
Average Rating = AVERAGE(‘sheet’ [Rating])

- Positive Reviews
Positive Reviews = CALCULATE( COUNTROWS(‘sheet’), 
‘sheet’[Sentiment]="Positive" )

- Negative Reviews
Negative Reviews =
CALCULATE(COUNTROWS(‘sheet’),
‘sheet’ [Sentiment]="Negative")

- Neutral Reviews
Neutral Reviews = CALCULATE( COUNTROWS(‘sheet’),
‘sheet’[Sentiment]="Neutral" )


## Dashboard Interaction
-<a href="https://github.com/janvipatil2601-oss/Amazon-Customers-Sentiment-Analysis-/blob/main/Dashboard.pbix">View Dashboard</a>

## Dashboard
![Screeshort(495)]( https://github.com/janvipatil2601-oss/Amazon-Customers-Sentiment-Analysis-/blob/main/Screenshot%202026-07-08%20184026.png)
