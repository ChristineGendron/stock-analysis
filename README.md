# Green Stocks Analysis
## Overview
This project is meant to provide a client with a tool that lets them analyze and compare the performance of a group of green energy stocks, in order to make recommendations.

## Results
### Conclusions about Market
Our analysis shows that, based on this sample of stocks, the performance of green energy securities decreased overall from 2017 to 2018. It also shows a high level of volatility, with some stocks increasing in value dramatically in 2017 before falling significantly in 2018. These investments would be best for someone with a relatively high tolerance for risk. 

### Outcome of Code Refactoring
This code initially used a nested For loop to iterate through every line of data twelve times (once for each ticker in the ticker index), outputting the ticker, volume, and returns for one stock per loop. This code was refactored to loop through each line of data only once, using conditionals to sort that data into arrays of tickers, volumes, and returns. Outputs could then be pulled from those arrays. 
This change increased the speed at which the macro ran, from over 1 second to a fraction of a second (as seen in the below images).

![2017 Original Runtime](/Resources/VBA_Challenge_2017_Original.png)
![2018 Original Runtime](/Resources/VBA_Challenge_2018_Original.png)

![2017 Runtime](/Resources/VBA_Challenge_2017.png)
![2018 Runtime](/Resources/VBA_Challenge_2018.png)

### Pros and Cons of Refactoring Code 

In this case, refactoring the code increased the speed that our macro ran, and made it possible to greatly scale up the amount of data our client can analyze and compare at once. Refactoring code can make code more practical, easier and more intuitive to read and understand, and more efficient to run. It can also introduce problems, since it is easy to break code that already works by making changes. I had to change several references in this code in addition to restructuring the loops, and it took some time and effort. However, the increased power of this tool is extremely valuable for the client’s business.  
