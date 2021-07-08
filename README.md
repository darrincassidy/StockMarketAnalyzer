# StockMarketAnalyzer

Tools for analyzing stock market data. In general, historical quote data is processed, and flags are generated for various reasons. When patterns emerge via flags, rules can be applied to the dataset. These rules can then be tested while trading in real time, and then adjusted with their results. 



Below is a big-picture look at how the application works. 

1. Java program provides methods to access Alpha-Vantage webservice. The webservice returns stock market data in real-time. The format of the data has multiple options (i.e daily, weekly, monthly).
2. The webservice returns the data as a JSON array.
3. Java program then processes the array, formats the data, and saves it to various MySQL tables (see documentation for detailed descriptions of these tables and what they do). 
4. To perform analysis on a given market securities, Java classes are used to extract flags and patterns. 
5. Next, the flags and patterns are used to create simple rules. These rules can apply to a specific securities, a specified group of securities, or to a market or markets in general. 
6. The generated rules are then tested in real time. These rules are given a value, which goes up and down based on their success/failure. 


Various Features

1. Automated data acquisition and formatting.
2. Dashboard for live simulation results.
3. Dashboard for active flags and active patterns.
4. Log for rules created and rules killed.
5. Hindsight trading (more on this is documentation).



Also

I realize this may not be applicable when it comes to market trading. This is more of a project to get my feet wet when it comes to machine learning, and to show prospective employers what my skillsets are. 

Any professionals with insight into stock market computing or automated investment, your insight or advice would be greatly appreciated!
