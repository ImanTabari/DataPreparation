
## **Task description**

Task is to read the datafile you are given into a pandas dataframe and follow the instructions.

- Read in the data into a pandas dataframe.
- Display the usual basic information (datatypes, names, non-null values for columns) about the dataframe.
- Display the dataframe.
- Find out what values occur under "Indicator Name".
- Set the name of the columns to the only value you found under "Indicator Name" (the columns and their labels remain the same!). (Apply the operation to your dataframe!)
- Create a new dataframe dfcode which contains the "Country Code" and "Country Name" columns of your original dataframe. You will continue working with your original dataframe, in what follows, though.
- Remove the "Country Code", "Indicator Name", "Indicator Code" columns. (Apply the operation to your dataframe!)
- Make the column "Country Name" the index of your dataframe. (Apply the operation to your dataframe!)
- Get rid of columns which contain no values. (Apply the operation to your dataframe!)
- Display the basic statistics by year, incl. minimal, maximal, mean, median, standard deviation values. (Make sure you display these values for all the years!)
- What can you conclude from the yearly descriptives? Answer in a markdown cell.
- Display the basic statistics by country, incl. minimal, maximal, mean, median, standard deviation values. (Make sure you display these values for all the countries!)
- Display the basic statistics of your previous by country-statistics (i.e., the mean of country means, etc.).
- Display the first thirty rows of your original dataframe after sorting by the values for the **last year** in **descending** order. (Do not apply sorting to your original dataframe, just display!)
- What are some of the conclusions you can draw from the data you displayed (e.g., about the "countries" in the data)?
- Calculate the difference between the (0-filled) values for the **years 2010 and 2000** by country, sort it in a **descending** order, and display the **first 30 rows**. What are some of the conclusions you could draw from what you see?
- Display the **mean** values by year as a percentage of the **maximal** values for that year (e.g., if the mean value for 1965 were 200, and the maximal for 1965 were 400, then for 1965, you should be displaying 50).
- Display the countries (not the subdataframe, just the countries!) where the values for *all* years are missing.
- Display the subdataframe with the countries whose final year's values are bigger than the **final** year values' mean.
- Load the "capital.json" file, and arrive at a dataframe capitaldf containing the **name, capital, iso2, iso3** information (these three should end up as the columns) for every country in it.
- Find the subdataframe of the dfcode dataframe you created earlier on where the "Country Code" value is **not** in the "iso3" column of capitaldf. Hint: look up and use the .isin pandas Series method. Store this subdataframe in the variable dfnocode. Display dfnocode and explain in a markdown cell what you see and what this could be used for.
- Now display the subdataframe of your main dataframe with the yearly data where the index (the Country Name) is **not** in the "Country Name" column of dfnocode.
