Lesson 2 - **Manipulating Data Frames in R**

1.	Which of the following commands will print the first 6 rows of a data frame users?
-   [ ]	**head(users)**
-   [ ]	summary(users)
-	select(users)
-	arrange(users)

2.	You’re doing some analytics on the ages of the typical customer for a company. They give you a data frame customers containing the information from the table below. If you want to ignore all of the PII (personal identifying information) and only select the ages from the data frame, which of the follow lines of code would you use?
-	customers %>%
filter(-age)
-	customers %>%
filter(age)
-	customers %>%
select(-age)
-	**customers %>%
select(age)**
