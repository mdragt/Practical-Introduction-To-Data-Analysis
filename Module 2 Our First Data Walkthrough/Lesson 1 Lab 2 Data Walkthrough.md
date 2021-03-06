# A Practical Introduction to Data Analysis for Absolute Beginners

## Module 2 - Lab 2: Data Walkthrough

## Learning Objectives

* Analyze a real-world data set.
* Find the average of one particular variable in a data set.
* Create a scatterplot in Excel showing the relationship between two variables.
* Compute the correlation coefficient in Excel between two variables.

## Data Set

[Car data set](Module%202%20Lab%20Real%20World%20Data%20-%20car%20data.xlsx)
This is the same data set as you used for the prior lab. In case you haven't done that lab, you can dowload the data file and store it on your local device. Then go to Excel Online, and open the corresponding data using the "Upload and Open..." option.

## What You’ll Need

To complete the lab, you will need the online version of Microsoft Excel.

## Overview

In this lab, we’ll sort variables, average variables, and explore the relationship between two different
variables using our car data from the lesson. We’ll also play around a bit with visualizing our data in a scatterplot.

### Exercise 1: Sorting and Averaging by Engine Size

1. Go to Excel Online and open the file from the prior lab.

Here’s a snapshot of the data:

![Cars data set](img/2020-06-15-14-03-15.png)

Once again, here’s what each variable/column represents:

* model = name of car model
* mpg = gas mileage, in miles per (US) gallon
* cyl = number of cylinders
* disp = displacement, in cubic inches
* hp = gross horsepower
* drat = rear axle ratio
* wt = weight, in thousands of pounds (1000 lb)
* qsec = 1/4 mile time
* vs = engine (0 = V-shaped, 1 = straight)
* am = transmission (0 = automatic, 1 = manual)
* gear = number of forward gears
* carb = number of carburetors

2. With the data set open, click anywhere in the spreadsheet, go to the Data tab in the ribbon, and click Filter (in the Sort & Filter tab). Probably, as you opened the file from the last lab, the filter option has already been activated.

![Filter](img/2020-06-16-09-28-13.png)

3. Click the arrow next to the number of cylinders (“cyl”), then click Sort Ascending to sort the cars by engine size (number of cylinders they have).

![Sorted by CYL](img/2020-06-16-09-58-52.png)

It seems that the cars in our data have engine sizes that range from 4 to 8 cylinders.

4. Now find the mean/average number of cylinders among the cars on this list. Start by creating a new column for this average, out to the right-hand side of the rest of the data.

![Create column](img/2020-06-16-10-01-35.png)

5. Use the AVERAGE function in Excel to find the mean/average number of cylinders. If you recall from our video lesson, the mean/average is just the sum of all the scores divided by the number of scores. Thankfully, Excel can crunch those numbers for us.

(Note: It’s not a requirement that you sort the data before averaging it. Sorting just makes everything easier to see.)

The syntax for Excel’s AVERAGE function is:

=AVERAGE(first cell:last cell)

Since you want the average number of cylinders, use column C as your range of data. You can either type in C2 as the first cell and C33 as the last cell, or you can just type in =AVERAGE( ), click inside the parentheses, and highlight all the cells from C2 down to C33. Once you hit Enter, the program will calculate the average for you from that column.

![Average CYL](img/2020-06-16-10-05-22.png)

So the average car from this data set had about 6.1875 cylinders.

### Exercise 2: Creating a Scatterplot

Next, we’ll create a graph in Excel that shows the correlation between two different variables. Let’s see
if there’s a correlation (relationship) between engine size and horsepower.

1. With the car data set open in Excel Online, highlight all of column C (“cyl”) and copy the data (Ctrl + c on Windows, Command + c on Mac). Paste the data into a new column, off somewhere to the right-hand side of the rest of the spreadsheet — we’re pasting it into column O in this
example.

![Copy CYL](img/2020-06-16-10-43-40.png)

2. Repeat Step 1 with column E (“hp”). Paste all the horsepower data into a column adjacent to then “cyl” data you just pasted. In this example, that’s column P.

![Copy HP](img/2020-06-16-10-46-08.png)

*Note: Excel Online doesn’t support selecting multiple non-adjacent cells or columns, which is
why we’re copying and pasting the two columns before creating the chart. If you have access to a desktop version of Excel, you can instead use Ctrl + click (or Command + click on a Mac) to select non-adjacent data and skip the copy/paste part.*

3. Select your two new adjacent columns of data (columns O and P). With both columns of data selected, click the Insert tab in the ribbon, then click Scatter > Scatter only with Markers.

![Add scatterplot](img/2020-06-16-10-49-42.png)

*Note: Again, if you’re using a desktop version of Excel instead of Excel Online, you can just select the two non-adjacent “cyl” and “hp” columns directly from the original data instead of copy/pasting.*

This should create a simple scatterplot showing the “cyl” (cylinder) data on the x -axis and the “hp” (horsepower) data on the y -axis, like so:

![Scatterplot](img/2020-06-16-10-52-26.png)

You’ll need to add some titles and legends to make the chart easier to read, though.

4. To add a better chart title, click on the scatterplot itself, then click Chart Tools in the ribbon and
go to Chart Title > Edit Chart Title.

![Edit title](img/2020-06-16-15-30-09.png)

Type in “Engine Size vs Horsepower” under Title Text, then click OK. Your scatterplot now has a shiny new title.

![Add title](img/2020-06-16-15-34-13.png)

5. Click into Chart Tools in the ribbon again, and click Legend > None to get rid of that little blue dot at the bottom that says “hp.”

![Remove legend](img/2020-06-16-15-36-25.png)

6. Finish up by adding titles to the x - and y -axis. To do this, head back to Chart Tools in the ribbon again, then click Axis Titles > Primary Horizontal Axis Title > Edit Horizontal Axis title. Type “Number of Cylinders” and hit OK.

![Add horizontal axis](img/2020-06-16-15-38-44.png)

7. Do the same thing for the vertical axis: Go to Chart Tools > Axis Titles > Primary Vertical Axis Title > Edit Vertical Axis Title. Type in “Horsepower” as the title and click OK.

![Add vertical axis](img/2020-06-16-15-40-39.png)

Now your scatterplot should be nice and easy to read.

![Final graph](img/2020-06-16-15-42-11.png)

You can see from the plot that there does seem to be a correlation between an engine’s number of cylinders and its horsepower. The higher dots on the right show that a higher number of cylinders usually means a higher horsepower. We call that a **positive correlation**.
