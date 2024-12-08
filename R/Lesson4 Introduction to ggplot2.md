Lesson 4 - **Introduction to ggplot2**

1.	What are the basic units in the grammar of graphics?
-  [ ]	Geometries and data.
-  [ ]	Aesthetics and geometries.
-  [x]	**The data, the aesthetics, and the geometries.**
-  [ ]	Data and layers.

2.	Which of the following statements about the ggplot() function is false?
-  [ ]	The ggplot() function is the first function call required to create any ggplot visualization.
-  [x]	**The ggplot() function maps data on the visualization.**
-  [ ]	The ggplot() function binds the data to the ggplot object, or the “canvas” of the graph.
-  [ ]	The arguments specified inside the ggplot() function are inherited by all of the subsequent layers.

3.	Which arguments in the labs() function would render the following plot?

    ![R lesson 4 - 1](https://github.com/damalialutfiani/Quizz-on-codecademy2/assets/74751990/7bf997fc-c868-41d9-97ae-9d28b0ae950b)

-  [ ]	labs(header="Monthly Rent vs Apartment Size in Brooklyn, NY", caption="Data by StreetEasy (2017)", x="Monthly Rent ($)", y="Apartment Size (sq ft.)")
-  [x]	**labs(title="Monthly Rent vs Apartment Size in Brooklyn, NY", subtitle="Data by StreetEasy (2017)", x="Monthly Rent ($)", y="Apartment Size (sq ft.)")**
-  [ ]	labs(title="Monthly Rent vs Apartment Size in Brooklyn, NY", subtitle="Data by StreetEasy (2017)", xlab="Monthly Rent ($)", ylab="Apartment Size (sq ft.)")

4.	Which of the following lines of code assigns color to the data on a scatterplot based on their genre value?
-  [ ]	ggplot(aes(color=genre))
-  [x]	**geom_point(aes(color=genre))**
-  [ ]	geom_point(color=genre)

5.	When is it best to use a scatterplot?
-  [ ]	If you want to show the variability of a dataset.
-  [x]	**If you want to inspect the correlation between two variables.**
-  [ ]	If you want to show the distribution of the dataset.

6.	Add a scatterplot layer to the viz ggplot object that colors the points based on the category variable.
___ + ___ (aes( ___ = ___ ))
-  [x]	geom_point
-  [x]	color
-  [x]	viz
-  [ ]	category

Click or drag and drop to fill in the blank

        viz + geom_point (aes( color = category ))

7.	What is the difference between manually setting aesthetics and providing aesthetic mappings?
   
