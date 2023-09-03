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
-   [x] **1**
-   [ ] 2
-   [ ]	Both

3.	The table below represents a data frame df that stores the exercises and repetitions of a workout routine. What piece of code would remove any duplicate rows from the data frame?
-   [ ]	df <- df %>%

        unique()
-   [ ]	df <- df %>%

        duplicated()
-   [ ] df <- df %>%

        remove_duplicates()
-   [x] df <- df %>%

        distinct()

4.	What do we use gather() for?
-   [ ]	Dropping duplicate values from a data frame
-   [ ]	Making the data frame smaller in size
-   [x]	**Reshaping a data frame into the rows and columns we want**
-   [ ]	Filling NA values in a data frame

5.	The table below represents a data frame df that stores a statistics final exam scores for a group of students. What would you need to do in order to analyze the students’ scores?
-   [ ] Convert exam_scores to a numeric type and then remove the % symbol using mutate() and gsub().
-   [x]	**Remove the % symbol using mutate() and gsub() and then convert exam_scores to a numeric type.**
-   [ ]	Convert exam_scores to a numeric type and then remove the % symbol using update() and substitute().
-   [ ]	Remove the % symbol using update() and substitute() and then convert exam_scores to a numeric type.

6.	What command do we use to see the types of data that each column in a data frame df holds?
-	types(df)
-	typeof(df)
-	**str(df)**
-	class(df)
