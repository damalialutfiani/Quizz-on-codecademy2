Lesson 3 - **Data Cleaning in R**

1.	Let’s say we have a data frame df representing the table below. What would the following code produce?

        df %>%
          transmute(year = str_sub(year_occurred,1,4),
            suffix = str_sub(year_occurred,5,6))

-   [ ]	An error because str_sub() does not work with data frame columns
-   [x]	**A data frame with column year containing the year as a number and column suffix containing AD or BC.**
-   [ ]	A data frame with column year containing AD or BC and column suffix containing the year as a number.
-   [ ]	A data frame with three columns: year_occurred, year, and suffix

2.	Which of these two data frames represent “tidy” data?
-   [ ]	Neither
-	**1**
-	2
-	Both