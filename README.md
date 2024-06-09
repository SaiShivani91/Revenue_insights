# Revenue Insights in Hospitality Domain using PowerBI

The main objective of this project is to create an interactive dashboard using PowerBI of the considered dataset through data loading, data transformation, data modelling and data visualization.

The techniques implemented in the project are listed below:

- Data Loading
- Power Query
- Data Modelling
- Data Analysis Expression (DAX)
- Dashbord Building

The tools implemented in the project are listed below:

- PowerBI

# Data Loading

The data is loaded into the PowerBI. The data is converted into table datatype. 

# Power Query

Power Query is mainly used for data cleaning or data transformation. Null values are removed in this. Some other column transformations are also performed.

# Data Modelling

Data modelling is mainly useful in establishing relation between various tables. The relation is established over here in the form of star schema. There are two types of tables in the considered data set. They are fact tables and dim tables. In this, the fact tables are placed in the middle and the dim tables are placed to surround them.

# Data Analysis Expression (DAX)

DAx is helpful in creating new columns andnew measures which will be useful in dashboard building. 
some of the DAX expressions used in the project are:

wn = WEEKNUM(dim_date[date])  


The above expression creates a new column consisting of week number.

var wkd = WEEKDAY(dim_date[date])

return if (wkd > 5, "Weekend", "Weekday")

The above expression returns the wkd value if it is greater than 5. 

Thus, the calculated columns and required calculated measures are created.

# Dashboard Building 

Different visualizations are created by employing different kinds of charts and data from all the tables. Finally, the interactive dashboard is built showing the key metrics and the key performance indicators (KPIs) enabling real time analytics and informed decision making.