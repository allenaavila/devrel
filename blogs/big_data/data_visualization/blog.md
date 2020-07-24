  
# How to Create a Tableau dashboard

**This blog will teach you how to create a Tableau dashboard in the following steps:**
* Step 1: Connect to a data source
* Step 2: Create a table with filters
* Step 3: Create a line graph with a date filter
* Step 4: Format the dashboard

Step 1: Connect to data source
- 
Please follow the link below to download Tableau. Fortunately, a 1-year free trial is available for students and teachers!

https://www.tableau.com/products/desktop/download

If you would like to download the data set I used, please follow the link below and select New_York_Times >> covid-19-county-level-data.csv and convert the csv file into an excel file.

https://www.kaggle.com/roche-data-science-coalition/uncover

Once you open Tableau, you need to connect to a data source. 
For this dashboard, we will use a Microsoft Excel file.

![](https://i.imgur.com/UUjUMPf.jpg)

After you have connected, you will find my raw data. I'm using data on COVID-19 cases by county here:

![](https://i.imgur.com/5o0HVof.jpg)



Step 2: Create a table with filters
- 
In the first sheet, we will create a COVID-19 stat table with state and county filters.
This step is broken into three parts:
* Create table
* Remove abc column
* Add filters

**1. Create table**

This is what you will see on the left side.
Dimensions displays Date, State, and County. Measures displays numeric columns, such as Cases and Deaths.

![](https://i.imgur.com/0GSeyCd.jpg)

In the table, we would like to display Date, State, County, Cases, and Deaths columns. So we will drag those column names into "Rows" section.

![](https://i.imgur.com/tLH334O.jpg)

But now the table looks weird because it thinks the values here are continuous.
To fix this, we need to set the columns labeled as Cases and Deaths to Discrete.

![](https://i.imgur.com/YIseNHc.jpg)

Once we change Cases and Deaths to Discrete, this is what it looks like!

This is almost what we want. There is still an Abc column, which will appear every time you create a table in Tableau. So, let's figure out how to remove the Abc column!

![](https://i.imgur.com/d3lQDWo.jpg)


**2. Remove Abc column**

This part will cover how to remove the Abc column step by step.
But if you would like to follow a video tutorial, feel free to check out the video below.

https://www.youtube.com/watch?v=6FTZ6TnYaF0

First, click any Abc column and click Format.

![](https://i.imgur.com/NZ6WGTx.jpg)

Change ***Default*** Pane color to White.

![](https://i.imgur.com/BcWDLzU.jpg)

This is what it looks like after you change the color.

![](https://i.imgur.com/ceout1e.jpg)

Choose the column on the left of Abc and click Format.

![](https://i.imgur.com/UqUSaab.jpg)


Under "Borders" — the grid icon to the right of the paintcan icon — set Column Divider Pane to None.

![](https://i.imgur.com/ZVc527t.jpg)

Lastly, shrink the width of the blank column. This is the final table!

![](https://i.imgur.com/nTLe6cI.jpg)

**3. Add filters**

Now, let’s add State and County filter. (You will need to choose "Select All" from List.)

![](https://i.imgur.com/OjVLHO0.jpg)

Right click on the State filter and choose "Show Filter."

![](https://i.imgur.com/xObIbNK.jpg)

This filter shows all of the states, but it's too lengthy!

![](https://i.imgur.com/yMBKQLd.jpg)

Right click the tiny dropdown in the State filter and change it to the form you like — I choose Single Value dropdown.

![](https://i.imgur.com/ENuRhRh.jpg)

Now, the lengthy filter list has changed to a dropdown list!

![](https://i.imgur.com/EPLT9LJ.jpg)

Change the title name, and this is the final product!

![](https://i.imgur.com/9YqW9RT.jpg)

To demonstrate what the last few steps provide here, let's apply a Georgia State filter on the right side and it displays the data for Georgia State only.

![](https://i.imgur.com/2qiWEI8.jpg)



Step 3: Create a line graph with a date filter
- 
In Sheet 2, we are going to draw a graph that displays the number of cases by each state.

Add Date as a column. The default is Year(Date). 

![](https://i.imgur.com/KBoRG6v.jpg)

Change Year to Exact Date. You can choose Month, Week Number, etc.

![](https://i.imgur.com/OySakLB.jpg)

Now, it shows the exact date you chose!

![](https://i.imgur.com/eb84ztv.jpg)


Let’s add #Cases to Rows to draw a graph!

![](https://i.imgur.com/NrJmp4B.jpg)

Now, let's apply a date range filter.
Add Date column to Filters and select “Range of Dates.”

![](https://i.imgur.com/TvTq1F7.jpg)

The range of dates automatically shows the range from start date to end date. Hit OK.

![](https://i.imgur.com/nOSmHtM.jpg)

Click the Date filter and select “Show filter.”

![](https://i.imgur.com/GPmQW1X.jpg)

Here we go! The date filter appears on the right side of the dashboard.

![](https://i.imgur.com/9qxEOry.jpg)

As mentioned earlier, we would like to display #Cases by state. Drag state dimension to Marks >> Color

![](https://i.imgur.com/EtVsmWf.jpg)

This warning pops up because the dataset contains 54 states, so we will apply a filter to select top states. Click “Filter and then add.” But if you would like to see all states, click “Add all members."

![](https://i.imgur.com/KUUBE5R.jpg)

Select California, Illinois, New Jersey, and New York, which are the states with most coronavirus cases.

![](https://i.imgur.com/osQETRU.jpg)

Tada!
The graph below displays COVID-19 cases by state.

![](https://i.imgur.com/0HDFtwb.jpg)

If you change the date range, the bar graph updates accordingly.

![](https://i.imgur.com/schpEg4.jpg)

If you would like to apply the date range filter to sheet 1 (COVID-19 case by State and County), you can do so by applying the date filter to all worksheets using the same data source. Once you do that, the date filter will be applied to both sheet 1 and sheet 2.

![](https://i.imgur.com/3XZuNIM.jpg)

Step 4: Format the dashboard
- 

In dashboard 1, drag sheet 1 to the blank page.

![](https://i.imgur.com/ORdHKDE.jpg)

Then you will notice that this dashboard does not have any space to display the bar graph we created in sheet 2. To fix this, we should expand the size of the dashboard. 

The default size is 1000 x 800 px. Let’s increase the height to 1600 px.

![](https://i.imgur.com/iLXt34y.jpg)

Select sheet 1 and click the downward arrow and select "Floating." This allows you to freely move the table and resize the table.

![](https://i.imgur.com/K25QOae.jpg)

Click “Floating” on the State and County filter as well and move them around as you would like.

![](https://i.imgur.com/eAg9Add.jpg)

Follow the same steps above and add sheet 2 to the dashboard.

![](https://i.imgur.com/NGeWYvY.jpg)

Now, let's add a title to the dashboard!

Select "Show dashboard title" in the Objects section and add the title.

![](https://i.imgur.com/hbZbZ1h.jpg)

The dashboard looks too plain, so let's add a background color to the title.

![](https://i.imgur.com/8Er750I.jpg)

Right click the title and click "Format title…"

![](https://i.imgur.com/YDKw8AU.jpg)

Apply Shading in the Dashboard Title section.

![](https://i.imgur.com/RsmLOhP.jpg)

Here is the final product of the dashboard!

![](https://i.imgur.com/dbwHZVE.jpg)

![](https://i.imgur.com/4Y8RT3m.jpg)

Feel free to check out the dashboard we just created! Play around with the date range filter, state, and county filter to see what happens!

https://public.tableau.com/profile/narae.lee#!/vizhome/COVID-19StatusDashboardatCountyLevel/Dashboard1?publish=yes

In this blog, we have learned how to connect to a data set, create a table and a line graph, and add different types of filters. As these features are the basics of data visualization, you can apply these features in any Tableau dashboard. 

If you would like to dive into Tableau further, I would recommend working with a more complicated dataset and looking into the following features:

1. Create a calculated field, which allows you to create a new column from data that already exists in your dataset
2. Work with maps in Tableau

Thank you for reading my blog!
