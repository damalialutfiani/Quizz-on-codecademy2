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
            summarize(number_of_unique_customers = n_distinct (name))

3.	A movie review website employs several different critics. They store these critics’ movie ratings in a data frame called movie_ratings, which has three columns: critic, movie, and rating. What command would give the average rating for each movie?

movie_ratings %>%
  _____  ( _____ ) %>%
    _____  (average_rating = _____ ( _____ ))

-	Movie
-	group_by
-	rating
-	summarize
-	calculate
-	mean
-	critic

Click or drag and drop to fill in the blank

movie_ratings %>%

  group_by(movie) %>%

 			summarize(average_rating = mean(rating))

4.	Grouping a data frame with group_by() and then piping the result into a filter() that uses summary functions allows you to:
-	filter rows of a data frame based on individual column values rather than per-group metrics
-	filter groups of a data frame based on per-group metrics rather than individual column values
-	**filter rows of a data frame based on per-group metrics rather than individual column values**
-	filter groups of a data frame based on individual column values rather than per-group metrics

5.	The City Library has several branches throughout the area. They collect all of their book checkout data in a data frame called checkouts. The data frame contains the columns location, date, and book_title. If we want to compare the total number of books checked out at each branch, what code could we use?

checkouts %>%
_____  ( _____ ) %>%
_____  (count = _____ )

-	Summarize
-	group_by
-	n()
-	date
-	location
-	book_title

Click or drag and drop to fill in the blank
   checkouts %>%
 		group_by(location) %>%
   
6.	Consider a data frame inventory for an athletics store with columns product and price.
