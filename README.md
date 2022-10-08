# All Stocks Analysis - Refactored

## Overview of Project

The next analysis was made in order to determine which of all the Tikcers in the given information regarding pro-energy companies is the best suitable option to aquire stock from. This was made using two primary parameters:
- Yearly return: the percentage the stock price grew or was reduced in the year. 
- Total Daily Volume: the sum of all the daily volumes.

Two Macros were built for this task, the first being a test version to achieve our initial goal, and the second version was built having the purpose of creating a more optimized and faster one and that gives the same results.  

## Results

###Stock Performance
- Regarding the stock performance results from both years 2017 and 2018 are really different, almost night and day. In the year 2017 we have an overall positive result in the return parameter, ***the only ticker that got a negative return is TERP***, while in 2018 ***only ENPH and RUN*** got a positive result. 


![VBA_Challenge_2017_re](https://user-images.githubusercontent.com/110573146/194690778-40df423b-9a00-4d1b-a12f-ed29f325091a.png)


![VBA_Challenge_2018_re](https://user-images.githubusercontent.com/110573146/194690787-69277f5f-eaf9-409b-a887-3dc354e0bd0f.png)


- So you can conclude that these two tickers of 2018 are the ones more likely to have a good result in the next year, but in order to determine which is the best to invest in we have to see the total volume of these and the percentage of the return. RUN in 2017 had a higher value in the volume but a lower percentage of return, while in 2018 the lower value in the volume stayed the return percentage was higher than ENPH. ENPH is a better option because in both years it had a higher value of volume and even though in 2018 it had a lower percentage it was only for 2% and added to that its consistency in high percentage also is a good signal, since RUN had only a 5.5% while ENPH a 129.5%. So it is far more appealing to have consistency in investments.

###Excecution Times
- Now talking about the time it took each version of the Macro we can say that it was totaly much more efficient and faster the refactored one. It gives all the correct information well formatted and in just a glimpse. Once we ran both Macros the differnece was evident and the pop up message confirmed it, the refactored one is almost 7 times faster. while the first version takes approx 0.73 seconds the second takes 0.11 seconds in comparisson.***This stays true for both years***


![VBA_Challenge_2017](https://user-images.githubusercontent.com/110573146/194691069-4eac8a74-da96-4a8a-8e7b-a03133eecf76.png)


![VBA_Challenge_2018](https://user-images.githubusercontent.com/110573146/194691073-3e0596a7-5675-4085-b6b3-09813b545593.png)


## Summary
1. What are the advantages or disadvantages of refactoring code?
Some disadvantages I found were:
- The refactoring tends to make longer the subroutine since it is separating tasks and creating more variables or arrays for the ocassion.
- More arrays were needed to solve the problem. 

The advantages it has are far more superior to the disadvantages though:
- It runs only 1 time through the info.
- It stores all the data separately and does not overwrite it for the arrays.
- It is faster.
- It uses less for loops to work.

2. How do these pros and cons apply to refactoring the original VBA script?
Pros:
- It run through all the rows just 1 time in comparison to the other one that runs through it 12 times, one for each ticker.
- As it does not do any repetitions reading through the info it saves a lot of time, 6 seconds (almost).
- All the values are saved in the arrays and can be accessed at the end without a fear of being overwritten and lost. 
- You only need to work with one for loop to cycle through the rows while the first used two for loops, one for the rows and the other for the index.
- It can even format the results sheet in the same subroutine.

Cons:
- 3 more arrays were necessary for the refactoring so a little more memory was needed.
- It is a little bit larger in size because of the new variables and the extra for loop needed to print the results at te end.
