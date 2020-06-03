# Assignment-04
This is the fourth assignment for BIOL390: Reproducible Research in the summer of 2020. The purpose of this assignment is to familiarize you with the creation and use of tidy datasets.

1) You will make a personal copy of this project by forking the repo.
2) You should then clone the forked repo on your remote to your local machine.
3) From there, you will work to complete the Assigment-04.Rmd file.
4) You are going to create your own dataset for this assignment.
	A) You will need to see 100 vehicles (observations), so head to the nearest parking lot!  
	B) For each vehicle, you will need to record the following variables:  
		i) Type (as a factor - e.g. Sedan, SUV, Pickup, Van, Truck, etc.)  
		i) Make (as a factor - e.g. Ford, Honda, Chevy, etc.)  
		i) Color (as a factor - e.g. Red, Green, Silver, etc.)  
		i) Sticker (as a logical - e.g. T or F, TRUE or FALSE, 1 or 0)  
	C) Make your dataset in whatever you want (Notepad, Excel, etc.)  
	D) Save your dataset as a csv file  
	E) Put a copy of your dataset in your assignment 4 folder
5) use `read_csv()` to import your dataset as a tibble where instructed.
6) If your data is tidy, you can use the tidyverse pipes to simplify analysis for the results section. `table <- yourTibble %>% group_by(variable) %>% summarize(Number = n()) %>% arrange(desc(Number))` creates a table with vehicles grouped by a variable and the number of each kind listed in decreasing order. The most common type will be at the top of the table. You can produce a nice html table from that if you use `knitr::kable(table) %>% kable_styling(full_width = F)`. You should do this for vehicle type, make, and color where indicated. Obviously, you need to change the variable names for 'table' and 'variable' as appropriate! Provide a caption for each table in the same way that you did for assignment 3.
7) You should also make some bar charts of the data where they are called for. `ggplot(myData, aes(x=variable, y=Sticker)), geom_bar(position = "dodge", stat = "summary", fun="mean")` should work to give you what you need. Make sure to use `fig.cap=` to set the figure captions and number them all sequentially (i.e. **Figure 1:** A plot of foo vs bar).
8) Finally, you need to add ANOVA analyses for each contrast. Borrow the code from prior assignments to help you to compare different variables to the proportions with stickers.
9) Make at least two commits of your different changes using git.
10) Push each of your commits up to your remote on GitHub.
11) Knit your final document and submit Assigment-04.html to Canvas.
12) Finally, create a pull request to submit your altered fork to me.

If you can do all that, you probably had a decent tidy data set and remembered your prior lessons with git. You are now ready to move on to meatier exercises. 
