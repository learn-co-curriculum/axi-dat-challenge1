# Mod 1 Code Challenge: Star Wars Starships

This assessment is designed to test your understanding of these areas:

1. Importing data
2. Data manipulation in SQL and/or Pandas
3. Creating visualizations using Matplotlib
4. Interpreting and communicating results of an analysis
5. (BONUS) Querying an API

Create a new jupyter notebook to complete the challenge and show your work. Make sure that your code is clean, readable and each step of your process is documented. For this challenge each step builds upon the step before it. If you are having issues finishing one of the steps completely, move on to the next step to attempt every section.

### Importing Data

Contained in this repo is a SQLite database named ***starwars_starships.db***. The name of the table is `starwars_starships`. Using SQL and/or Pandas import the data contained in this database to begin data cleaning and analysis.

### Data Cleaning and Filtering

* Once you have your data your tasks are to:
* Select only rows that do not have 'unknown' in the length column
* Change the datatype of the `cost_in_credits` and `length` columns to floats
* Create a new column `cost_per_length` which is calculated by `cost_in_credits` / `length`
* Create a dataframe which includes only the ***5 starships*** with the ***highest*** `cost_per_length` in ***descending*** order

### Visualization

After cleaning your data and filtering for the appropriate people, create a bar graph which will visualize the `credits_per_length` of the five starships. Use the `name` of the starship as the label for each bar. This visualization should contain:
* An informative title
* Labeled axes
* An appropriate scale

### Communicating Results
For the last portion of the challenge imagine that you are looking to purchase a starship and want to get the longest ship for the best price. Write a short paragraph describing the information you have distilled and note any interesting trends or anomalies in the data that would help you decide what starship is right for you. 

### (Bonus) API: Finding the Pilots

NOTE: Please do not atempt this section until you have fully completed the main sections

Using the requests library and the swapi [documentation](https://swapi.co/documentation), use the urls found in the pilots column to find the name of the pilot for the 5 starships in your final dataframe and add them to your final dataframe in a column called `pilot_name`. If there is no pilot available for a particular starship simply add the value of ‘no pilot’ instead.

# Deliverables
Your main deliverable is a jupyternotebook containing the following clearly labeled:
1. A pandas dataframe with only the starships with the top 5 highest `credits_per_length` in descending order with only the name and `credits_per_length` column. If you completed the BONUS section also include the `pilot_name` column.
2. A bar graph visualizing each of the top 5 starships with their corresponding `credits_per_length`
3. A short paragraph detailing your rational for what is the best starship to purchase based on your analysis