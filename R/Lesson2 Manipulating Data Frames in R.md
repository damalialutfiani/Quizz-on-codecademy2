Lesson 2 - **Manipulating Data Frames in R**

1.	Which of the following commands will print the first 6 rows of a data frame users?
-   [x]	**head(users)**
-   [ ]	summary(users)
-   [ ]	select(users)
-   [ ]	arrange(users)

2.	You’re doing some analytics on the ages of the typical customer for a company. They give you a data frame customers containing the information from the table below. If you want to ignore all of the PII (personal identifying information) and only select the ages from the data frame, which of the follow lines of code would you use?
-   [ ] customers %>%

        filter(-age)
-   [ ]	customers %>%

        filter(age)
-   [ ]	customers %>%
        
        select(-age)
-   [x]	customers %>%

       	select(age)

3.	The table below represents a data frame attendance which stores attendance data for students at a high school. What piece of code would create a new data frame containing student names and the total number of days absent or late?
-   [ ]  attendance %>%

        transmute(total_absent_late = days_absent + days_late)
-   [ ]  attendance %>%
        
        mutate(total_absent_late = days_absent + days_late)
-   [x]  attendance %>%
 	
        transmute(student_name = student_name,
  
          total_absent_late = days_absent + days_late)
-   [ ]  attendance %>%

        mutate(student_name = student_name,

          total_absent_late = days_absent + days_late)

4.	You import photo data from a social media website into a data frame photos. The three columns are photo_id, likes, and comments, representing the unique photo identifier, the number of likes on a photo, and the number of comments on a photo, respectively. What piece of code would you use to update the name of the likes column to num_likes and the comments column to num_comments?
-   [x]	photos %>%

        rename(num_likes = likes, num_comments = comments)
-   [ ]	photos %>%

        colnames(num_likes = likes, num_comments = comments)
-   [ ]	photos %>%
        
        rename(likes = num_likes, comments = num_comments)
-   [ ]	photos %>%
        
        colnames(likes = num_likes, comments = num_comments)

5.	Which of the following commands will correctly import the file content_inventory.csv into a data frame content?
-   [x] **content <- read_csv('content_inventory.csv')**
-   [ ] content <- read_csv('content_inventory')
-   [ ] content <- from_csv('content_inventory.csv')
-   [ ] content <- from_csv('content_inventory')

6.	The table below represents a data frame grades that contains students’ scores for 3 units in a Biology course. What piece of code would order the rows of the data frame by the unit 3 scores, in descending order?
-	grades %>%
order_by(unit_3)
-	grades %>%
arrange(unit_3)
-	**grades %>%
arrange(desc(unit_3))**
-	grades %>%
order_by(desc(unit_3))
