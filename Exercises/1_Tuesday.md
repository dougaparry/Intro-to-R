# Tuesday Exercises

This session is based around chapter 5 of the book R 4 Data Science. It is important that you work through the chapter completely to understand all of the important concepts (both those covered in the session and the rest covered in the chapter). Afterwards, we have extracted a number of relevant exercises from the chapter to work through. For these exercises you can use the provided notebooks and data at: https://github.com/dougaparry/Intro-to-R to get started (download the full repository as a zip file to access the files on your computer). While the solutions for the exercises can be found on the Internet and in the drive, we encourage you to work through the exercises using the chapter first to get used to solving problems with R.

- Chapter: 5 https://r4ds.had.co.nz/transform.html 

__Exercises:__

1. Find all flights that
    1. Had an arrival delay of two or more hours
    2. Flew to Houston (IAH or HOU)
    3. Were operated by United, American, or Delta airlines.
    4. Departed in Winter (July, August, and September)
    5. Arrived more than two hours late, but didn’t leave late
2. How many flights have a missing dep_time? What other variables are missing? What might these rows represent?
3. Use the `arrange()` function to sort all missing values to the start of the dataset? (Hint: use `is.na()`).
4. Sort flights to find the most delayed flights. Find the flights that departed the earliest.
5. Which flights travelled the farthest? Which travelled the shortest?
6. What happens if you include the name of a variable multiple times in a `select()` call?
7. Currently `dep_time` and `sched_dep_time` are convenient to look at, but hard to compute with because they’re not really continuous numbers. Convert them to a more convenient representation of number of minutes since midnight.
8. Compare `air_time` with `arr_time` - `dep_time`. What do you expect to see? What do you see? What do you need to do to fix it?
9. Look at the number of cancelled flights per day. Is there a pattern? Is the proportion of cancelled flights related to the average delay?
10. What does the `sort` argument to `count()` do. When might you use it?
11. Which plane (tailnum) has the worst on-time record?
12. What time of day should you fly if you want to avoid delays as much as possible?
13. For each destination, compute the total minutes of delay. For each flight, compute the proportion of the total delay for its destination.
14. Delays are typically temporally correlated: even once the problem that caused the initial delay has been resolved, later flights are delayed to allow earlier flights to leave. Using lag(), explore how the delay of a flight is related to the delay of the immediately preceding flight.
15. Look at each destination. Can you find flights that are suspiciously fast? (i.e. flights that represent a potential data entry error). Compute the air time of a flight relative to the shortest flight to that destination. Which flights were most delayed in the air?
