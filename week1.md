# Basic Pandas warm up
Read in [this dataset](https://s3.amazonaws.com/python-level-2/sales-funnel.csv) and answer the following:

0. What is this dataset?
1. What insights do you want to extract from it?

Then write code to answer the following:

0. How many rows have a price greater than $8,000?
1. How many rows are pending AND have a price greater than $8,000?
2. How many rows are pending OR have a price greater than $8,000?
3. Create an amount column that's equal to price * quantity. What's the total amount won?
4. What's the total amount won within the CPU product category?

**HINT**: Look for boolean masks or filtering within a Pandas data frame. 

# Reshaping dataframes
## Pivot tables
0. Google `pandas pivot_table` and look at the docs.
1. What's a pivot table for?
2. Let's play around with the pivot_table function call and see what it does.

Creative exercise: Come up with pivot tables you would find useful. 

## Groupby
0. Let's Google `pandas groupby` and look at the docs and a few examples.
1. Let's group on status and aggregate using the `np.sum` function.

Exercise
Achieve the same output using a pivot table.

# Working with Text Data
0. Let's go to the `pandas` docs section on working with text data.
1. Let's use `.str...` to select the rows that contain either pending or won.
2. Let's lowercase the Rep column with `.str.lower`

Exercises:

0. Replace the product category `CPU` with `monkey`
1. Upper case the product category column.
2. Create a new column called "contains_monkey" using `str.contains` based on the product category value.

# Practice on new dataset
## Solo
0. Read in [this dataset](https://raw.githubusercontent.com/suneel0101/lesson-plan/master/crunchbase_monthly_export.csv). What is it?
1. What is the max funding total? (Hint: may have to clean/convert that column; check dtypes)
2. Rename the columns so they're reasonable.
3. Create a pivot table of market against total funding, sorted from highest to lowest and only include the top 10.
4. How many companies contain the Game category?
5. What is the average funding total of companies from the city `New York`? How about `San Francisco`? How do they compare?
6. Get descriptive statistics on the dataset (good to do this at the beginning of your analysis).
