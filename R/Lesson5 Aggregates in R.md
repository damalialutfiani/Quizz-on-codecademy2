Lesson 5 - Aggregates in R

1.	Grouping a data frame with group_by(), piping the result into a call to mutate(), and defining new columns in terms of summary functions allows you to:
-	create a new data frame that contains one row for each group a new column with per-group metrics
-	**add new columns to a data frame that are based on per-group metrics**
-	add new groups to a data frame that are based on per-column metrics
-	create a new data frame that contains one column for each group a new row with per-group metrics

2.	You are working for an online retailer of mechanical keyboards and have access to the customer_purchases data frame. In this data frame there is a row for each purchase a customer has made on the site. If the customers’ names are stored in a column called name, what command would you use to determine how many unique customers purchased something from the site?

customers %>%
 		summarize(number_of_unique_customers = _______ (name))

-	n_distinct
-	count
-	unique
-	distinct

Click or drag and drop to fill in the blank
customers %>%
 		summarize(number_of_unique_customers = n_distinct(name))
