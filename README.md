# ETLproject

E

One of the data sets we chose was from the CDC on the impaired driving death rate by state in 2012. We downloaded a CSV file of this data. The next data set we used was a ranking of the states by their alcohol consumption in gallons. This data set was created for an article using data from the National Institute on Alcohol Abuse and Alcoholism. This was also a CSV file.

T

The consumption data was simple and only had two columns. We just renamed the column headers to ‘state’ and ‘volume’ from ‘State’ and alcoholConsumptionGallons.’ This data frame was renamed to “consumption”

The CDC data set came with more data than we needed. We dropped all the columns we didn’t need and kept only ’State’ and ‘All Ages, 2012’. The  data set had columns for gender and age group. We called this final data frame, “impaired_clean” We had to rename “State “ to “state” because of the extra space in the original column heading.

L

We decided to use a declarative base instead of an automap. We originally wanted to do an automap base so it would create the database for us. We created the classes to serve as an anchor point for our tables. Here we defined the columns and what dtype would live there. After that we created the engine. Next we created a for loop to go through the data frames we created earlier. This filled the database.
