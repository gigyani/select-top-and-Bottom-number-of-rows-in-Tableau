# select-top-and-Bottom-number-of-rows-in-Tableau
I will show the method and then you can use those calculations in your workbook. 
First create a [Top & Bottom] parameter as Integer datatype and the select range in the Allowable Values.
Take values based on you requiremnets.
Then create a Calculated field and paste the code given below.
RANK( SUM( [Sales] ), 'desc' ) <= [Top & Bottom].
OR
RANK( SUM( [Sales] ), 'asc' ) <= [Top & Bottom]
This will create a T/F filter
Drag the T/F filter into the filters shelf and select True
Use parameter for the number of top and bottom values that you want
Arrange the values as ascending order
you can now see the top and bottom number of rows from a metric
Thanks
