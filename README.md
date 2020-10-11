# Stock-Analysis Using VBA

# Overview of Project
## Purpose of the Project

As part of an assignment for the UT Data Boot Camp, an initial stock analysis was conducted for Steve.  The original code was then refactored to loop only once.  The purpose is to determine if the refactored changes made an impact on the run time.  

Using run buttons, Steve will have the ability to put in the year into an input box, which removes any magic numbers.   The VBA code uses a timer, arrays, if-then conditional statements, assigns long/string data types, and adds static/conditional formatting.

# Results
## Comparing 2017 and 2018 Stock Analysis
Comparing the 2017 and the 2018 stocks, the difference in the total daily volume between the two years that resulted in less than a $100,000,000 in increased volume was not enough to generate a positive 2018 return percentage.  The tickers ENPH and RUN had would have been considered good investments due to the positive returns in 2018, and both of the tickers had increases greater than $200,000,000 over the 2017 total daily volumes. 
 
![Pic 1](https://github.com/Baylex/stock_analysis/blob/main/Resources2/1Compare_2017_2018.PNG)

## Comparing the Original Run Times to the Refactored Run Times

Run times for the original code took around .4 seconds.

![Pic 2](Resources2/2Original_2017_small.png)
![Pic 3](Resources2/3Original_2018_small.png)

Run times for the refactored code took around .08 seconds, which is displayed in scientific notation: 8 E -02.  
![Pic 4](Resources2/4New_2017_Refactored_small.png)
![Pic 5](Resources2/5New_2018_Refactored_small.png)

Refactoring the code did make the run times decrease, which optimizes the code. 

## What was the difference in the codes? 
The original code contained a nested for loop.  Included in that outer loop, it also output the data for the current data, which resulted in a significant number of iterations.  

![Pic 6](https://github.com/Baylex/stock_analysis/blob/main/Resources2/6Original_Code.PNG)

With refactoring the code to only have one loop and moving the output to a separate loop, the number of iterations was drastically reduced.

![Pic 7](https://github.com/Baylex/stock_analysis/blob/main/Resources2/7Refactored_Code.PNG)

# Summary
## 1. What are the advantages or disadvantages of refactoring code?
### Advantages
Finding the root cause of a potential bug can be done with refactoring.  A programmer can catch duplicated subroutines, unnecessary loops, redundant statements, or code that was used to run down an error but was accidently left in the script.  Another advantage is when a peer reviews another programmer’s work, they will come with a fresh perspective and can tidy up the code to make it run leaner. 

### Disadvantages

Programming can have multiple approaches to a solve a problem.  In those differences, programmers may have alternative logic steps, which will require testing to see how those differences play out in the script.  Refracting a stable code to apply a different set of logic could be costly or introduce new bugs into the system.  When juggling tight deadlines, programmers may also have to choose between refactoring or developing new code.  
	
## 2. How do these pros and cons apply to refactoring the original VBA script?
Reducing the number of loops decreases the memory needed for processing the data, which reduces the run time and optimizes the performance of the script. To refactor the code, testing has to be done with each new addition to check for the efficiency of the new code.  

