# coursera-de-c2-lab1-linux
Using Linux Lab

## Goal:  Truncate file with Bash

For this project you will create a shell pipeline that truncates a file via random shuffling, then verifies the correct number of lines.  Many times large files are so big that traditional data science libraries like `pandas` or `jupyter` cannot process them. One approach to dealing with this problem is to sample the file by truncating and shuffling the results.

### Part 1: Count the lines in the file and inspect the contents

1.  Run `wc -l nba_2017.csv`
2.  How many lines are in the file?
3.  Run the `head nba_2017.csv` and inspect the first few rows of the file.

### Part 2:  Truncate and shuffle the file

1.  Truncate and shuffle the file `shuf -n 100 nba_2017.csv > small_nba_2017.csv`
2.  Count the number of lines.  How many are there?
3.  If you inspect the first few lines what do you see?  `head nba_2017.csv 

### Part 3:  Remove Column Names Before Shuffle

1.  What happens when you run `tail -n +2 nba_2017.csv | head`?
2.  How could use this approach to remove the column heads before shuffling?
3.  Why would want to do this and how could you append them back on after you shuffle?