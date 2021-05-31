# Thursday Exercises

This session is based around chapters 14, 15, 16, and 20 of the book R 4 Data Science. It is important that you work through the chapters completely to understand all of the important concepts (both those covered in the session and the rest covered in the chapter). Afterwards, we have extracted a number of relevant exercises from the chapter to work through. For these exercises you can use the provided notebooks and data at: https://github.com/dougaparry/Intro-to-R to get started (download the full repo as a zip file). While the solutions for the exercises can be found on the Internet, we encourage you to work through the exercises using the chapter first to get used to solving problems with R.

- Chapter: 14 https://r4ds.had.co.nz/strings.html 
- Chapter: 15 https://r4ds.had.co.nz/factors.html 
- Chapter: 16 https://r4ds.had.co.nz/dates-and-times.html 
- Chapter: 20 https://r4ds.had.co.nz/vectors.html 

Exercises:

1. In code that doesn’t use `stringr`, you’ll often see `paste()` and `paste0()`. What’s the difference between the two functions? Which stringr function are they equivalent to? How do the functions differ in their handling of NA?
2. Use `str_length()` and `str_sub()` to extract the middle character from a string. What will you do if the string has an even number of characters?
3. What does `str_trim()` do? What’s the opposite of `str_trim()`?
4. Given the corpus of common words in `stringr::words`, create regular expressions that find all words that:
    1. Start with “y”.
    2. End with “x”
    3. Are exactly three letters long. (Don’t cheat by using str_length()!)
    4. Have seven letters or more.
    5. Start with three consonants.
    6. Have three or more vowels in a row.
    7. Have two or more vowel-consonant pairs in a row.
5. Use the built in General Social Survey (GSS) described in the video
    1. What is the most common relig in this survey? What’s the most common partyid?
    2. Which relig does denom (denomination) apply to? How can you find out with a table?

