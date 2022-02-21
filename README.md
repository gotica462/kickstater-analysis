# Kickstarting with Excel

## Crowfunding Analysis

 We want to determine how different fundraising campaigns fared in relation to their launch dates and their funding goals. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

  In order to do our analyisis first we have to summarize our data using a pivot table using the date the fundraising was launched. We want to know the outcome of those fundraising based on the launch date, amd we also need to filter the parent category that we are interested in, which in our case is theater. 
(see below images for the results)

![image](https://user-images.githubusercontent.com/99451833/154867672-70e82b47-7fed-41b8-8a41-4013d0174e7d.png)

![image](https://user-images.githubusercontent.com/99451833/154864221-5cf89631-6ca0-494f-9de6-4c227621db9d.png)

### Analysis of Outcomes Based on Goals

For our analysis based on goals, we want to know the percentage of succes or failure in the fundraising's campaigns based on the money asked. We only want to know the percentage of those fundraisings pertaining to the subcategory "plays". In order to do that we need to create a table with the ammmount of money of our goals and then use the COUNTIF() function in excel to determine the number of plays in that ammount range. Then, we can calculate the percentages on each of those range (See table below)

![image](https://user-images.githubusercontent.com/99451833/154868179-34310fc8-d1b9-4fdd-a889-ff7937856396.png)

We will use a line chart to better illustrate our results.

![image](https://user-images.githubusercontent.com/99451833/154868245-b30c1f25-7d97-4133-85d3-d77ec5335caa.png)

### Challenges and Difficulties Encountered

 One of the challenges we encountered was that the data for parent/category was together in one column, and for the purposes of our analysis we need it to split it into two separate columns of Parent and Subcategory to get additional insight. This was accomplished by using the "Text to Columns" and "Convert text to Columns Wizard" in excell.

Another challeng presented was that the launch at column was in Unix Timestamps, so we use the formula "=(("Column_Launched at"/60)/24) + DATE (1970,1,1)  to convert it to day-month-year format.
  
  ## Results
 
 Based on our data analysis we can conclude that those fundraising campaigns that launched between May and July tend to be more succesful than the other months, so we could suggest to start our campaign in the summer months.

We can also determine that December is the worst month to start a findraising campaign, since the percentage of failed/succesfull campaigns is almost the same. We can also determine that those campaign's "canceled" average the same throught out every month, so thos campaigns does not affect our analyisis.

  In our Oucomes based on Goals analysis for plays, we can determine that the more succesfull campaigns are those were the goal is between 0 and 5000, and if the range of the ammount of money for the goal increases, so does the likelihood that fundtraising will fail.  In simple terms, the more money is needed the less likey is the campaign to succeed. 
  
   One of the limitations in our Data for succesful campaigns based on Goal is the number of fundraising campaigns is that we do not have enough data in some ranges to do a proper analyisis. If we take a look at the table for our analyisis, we see that we only have 6 total projects in the range of 35,000 to 44,999. Not enough to do an analyisis. We could overcome this limitation by grouping our goal ammount ranges differently. For example only use the range of 25,000 or more.
  
   If we want to dig deeper into our data analyisis, we could also do a Pivot Table and a graph using the country as the filter. Are fundraising more succesfull in the US? in Great Britain? How many more campaigns are done in the Us than in Great Britain? 
  
 Also recommended, is to do a graph for the number of backers and how much they each pledge? is the goal ammount related to then number of backers? What is the average donated by  each backer? Another table that would be useful is to create a table and a graph to see how the data is distributed by looking at The three key measures of central tendency: mean, median, and mode. Are there any data outliers that affecting our results? What is the ammount of money that they pledge that is more repeated in our database? The answers to those question would give us a better understanding of the data so we can plan a succesfull fundraising campaign.


