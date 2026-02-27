Lesson 6 - Joining Tables in R

1.	Which of the following best describes a full join?
   -	A join where all rows are included, whether they match or not.
   -	A join where all rows from the second data frame are included, but only matching rows from the first data frame
   -	A join where all rows from the first data frame are included, but only matching rows from the second data frame.
   -	A join where only matching rows are included.
2.	Consider two data frames vets and appointments that store the appointment and vet data for a veterinarians office. vet has two columns:
the id and the name of the veterinarian, while appointments has three columns: the vet_id of the veterinarian holding the appointment,
the time of the appointment, and pet_owner_name.
Complete the code below to join the two data frames and keep only the matching rows.

joined_dfs <- vets %>%
      _____ ( _____ ,
            by = _____ )

-	full_join
-	right_join
-	c('id' = 'vet_id')
-	inner_join
-	c('vet_id' = 'id')
