# Friday Exercises

In addition to using the two open books (Fundamentals of data visualistion and Data Visualisation A practical introduction) this session is based around chapters 3 and 28 of the book R 4 Data Science. It is important that you work through the chapters completely to understand all of the important concepts (both those covered in the session and the rest covered in the chapter). Afterwards, we have extracted a number of relevant exercises from the chapter to work through. For these exercises you can use the provided notebooks and data at: https://github.com/dougaparry/Intro-to-R to get started (download the full repo as a zip file). While the solutions for the exercises can be found on the Internet, we encourage you to work through the exercises using the chapter first to get used to solving problems with R.

- Chapter: 3 https://r4ds.had.co.nz/data-visualisation.html
- Chapter: 28 https://r4ds.had.co.nz/graphics-for-communication.html 

Exercises: 
1. Make a scatterplot of `hwy` vs `cyl`.
2. What happens if you make a scatterplot of `class` vs `drv`? Why is the plot not useful? What happens if you use `geom_count()` instead?
3. What’s gone wrong with this code? Why are the points not blue?

`ggplot(data = mpg) +   geom_point(mapping = aes(x = displ, y = hwy, color = "blue"))`

4. Map a continuous variable to color, size, and shape. How do these aesthetics behave differently for categorical vs. continuous variables?

5. What happens if you map the same variable to multiple aesthetics?
6. What does the stroke aesthetic do? What shapes does it work with? (Hint: use ?geom_point)
7. What happens if you map an aesthetic to something other than a variable name, like aes(colour = displ < 5)? Note, you’ll also need to specify x and y.
8. What plots does the following code make? What does . do?

`ggplot(data = mpg) + geom_point(mapping = aes(x = displ, y = hwy)) + facet_grid(drv ~ .)`

9. Run this code in your head and predict what the output will look like. Then, run the code in R and check your predictions.

`ggplot(data = mpg, mapping = aes(x = displ, y = hwy, color = drv)) + geom_point() + geom_smooth(se = FALSE)`

10. What does the `se` argument to `geom_smooth()` do?
12. What does `geom_col()` do? How is it different to `geom_bar()`?
13. Create one plot on the fuel economy data with customized title, subtitle, caption, x, y, and colour labels.
