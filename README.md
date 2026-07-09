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

## Project Insights
### Sentiment Distribution
-	Most customer reviews are Positive.
-	Negative reviews represent a smaller percentage.
-	Neutral reviews indicate average customer satisfaction.

### Product-wise Sentiment
- Electronics and Home products receive the highest number of positive reviews. 
- Some categories show higher negative sentiment due to product quality or delivery issues.
- Positive sentiment dominates across most product categories.

### Rating Distribution
- Most customers give 4-star and 5-star ratings.
- Very few customers provide 1-star ratings.
- Higher ratings indicate overall customer satisfaction.

### Reviews Over Time
- Customer reviews increase during festive seasons and promotional sales.
- Review activity remains consistent throughout the year.
- Positive reviews generally increase with higher sales periods. 

### Verified Purchase Analysis
- Most reviews come from verified purchasers.
- Verified purchase reviews are generally more reliable.
- Positive sentiment is higher among verified buyers. 

### Review Length Analysis
- Longer reviews usually provide detailed customer experiences.
- Short reviews are mostly simple positive or negative feedback.
- Detailed reviews often receive more helpful votes. 

### Helpful Votes Analysis
- Reviews with more helpful votes provide detailed product information.
- Highly helpful reviews influence purchasing decisions.
- Positive reviews generally receive more helpful votes.

## Final Conclusion 
The Amazon Customers Sentiment Analysis Dashboard helps understand customer opinions through review analysis. Most customers are satisfied with products, as shown by the high number of positive reviews and ratings. Negative reviews mainly highlight issues related to product quality and delivery. The dashboard provides valuable insights into customer feedback and product performance. These insights help businesses improve customer satisfaction and make better decisions.


