Lesson 3 - **Data Cleaning in R**

1.	Let’s say we have a data frame df representing the table below. What would the following code produce?

df %>%
  transmute(year = str_sub(year_occurred,1,4),
