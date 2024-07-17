# Business Analytics Project E commerce
https://docs.google.com/spreadsheets/d/1LeNtroyjfjV-tgn9jIzNkMgwkKWffCA0whv6myZxHNo/edit?gid=38637670#gid=38637670

Build funnels and cohorts, gain insights, and provide recommendations.

The dataset has the following columns:
-	user_id: unique customer IDs
-	event_type: the type of activity by the user
-	category_code: category of the product being viewed or purchased
-	brand: company that makes the product
-	price: price of the product, in USD
-	event_date: date of the user activity, in YYYY-MM-DD format

In the first part, a conversion funnel was built to understand how well the website was converting product page views into purchases. Using the "raw_user_activity" sheet, a pivot table named "conversion_funnel" was created to count unique users at each stage of the funnel, which included three stages. Formulas were used to add columns for total conversion rates and conversion rates to the next step. This helped in visualizing the user interactions and identifying areas for improvement in the conversion process.

For the cohort analysis, data preparation was the key focus. Purchases were filtered from the "raw_user_activity" sheet and copied into a new "purchase_activity" sheet. A pivot table was created to calculate the minimum event date for each user, which was then used to determine the first purchase date for each user in the "purchase_activity" sheet using a VLOOKUP() function. Three new columns, event_month, first_purchase_month, and cohort_age, were created using the TEXT() and DATEDIF() functions to group users and transactions by month for the cohort analysis.

In the final steps, retention rates were calculated by grouping the data into cohorts based on the month of the first purchase. A pivot table named "cohort_analysis" was configured to count unique users for each cohort_age. A new sheet called "retention_rates" was created to calculate and display retention rates for each cohort month by month, excluding the first month. The entire spreadsheet was then organized and documented, with an executive summary sheet summarizing the results and analysis, and a table of contents for easy navigation. Formatting was applied for readability and presentation quality, ensuring the project looked polished and professional.


![Screenshot 2024-07-17 121246](https://github.com/user-attachments/assets/07f704bb-496b-4bbc-b5e0-606450d171df)
