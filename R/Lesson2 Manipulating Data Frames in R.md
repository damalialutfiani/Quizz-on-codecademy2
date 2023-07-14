Lesson 2 - **Manipulating Data Frames in R**

1.	Which of the following commands will print the first 6 rows of a data frame users?
-   [x]	**head(users)**
-   [ ]	summary(users)
-   [ ]	select(users)
-   [ ]	arrange(users)

2.	You’re doing some analytics on the ages of the typical customer for a company. They give you a data frame customers containing the information from the table below. If you want to ignore all of the PII (personal identifying information) and only select the ages from the data frame, which of the follow lines of code would you use?
-   [ ]         customers %>%

                  filter(-age)
       	
-   [ ]	        customers %>%

                  filter(age)
-   [ ]	customers %>%
        
                  select(-age)
-   [x]	**customers %>%
                  select(age)**

3.	The table below represents a data frame attendance which stores attendance data for students at a high school. What piece of code would create a new data frame containing student names and the total number of days absent or late?
-   [ ]  attendance %>%

        transmute(total_absent_late = days_absent + days_late)
-   [ ]  attendance %>%
        
        mutate(total_absent_late = days_absent + days_late)
-   [ ]  **attendance %>%
 	
  transmute(student_name = student_name,
  
total_absent_late = days_absent + days_late)**
-   [ ]  attendance %>%

mutate(student_name = student_name,

total_absent_late = days_absent + days_late)
