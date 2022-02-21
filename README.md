# Kickstarting with Excel

## Crowfunding Analysis

 We want to determine how different fundraising campaigns fared in relation to their launch dates and their funding goals. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

In order to do our analyisis first we have to summarize our data using a pivot table using the date the fundraising was launched. We want to know the outcome of those fundraising based on the launch date. We also need to filter the parent category that we are interested in, which in our case is theater. 
(see below images for the results)

![image](https://user-images.githubusercontent.com/99451833/154867672-70e82b47-7fed-41b8-8a41-4013d0174e7d.png)

![image](https://user-images.githubusercontent.com/99451833/154864221-5cf89631-6ca0-494f-9de6-4c227621db9d.png)

### Analysis of Outcomes Based on Goals

For our analysis based on goals, we want to know the percentage of succes or failure in the fundraising's campaigns based on the money asked. We only want to know the percentage of those fundraisings pertaining to the subcategory "plays". In order to do that we need to create a table with the ammmount of money of our goals and then use the COUNTIF() function in excel to determine the number of plays that were succcesful or failed in that ammount range. Then we can calculate the percentages on each of those ammount's range (See table below)

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
  
  


- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
