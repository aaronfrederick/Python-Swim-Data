# Python-Swim-Data
Cleans swim meet data and visualizes, analyzes features, and outputs a dataframe for visualization in R

This program takes the somewhat messy output that swim coaches get, reorganizes the swims, removes the irrelevant data, and finishes analysis.  It is broken up in a Jupyter Notebook into the following sections:
1) Definitions and Excel reading

2) Creates 3 dataframes:
  - All swims normalized by percent
  - All swims with time measured in the change of seconds from the first swim
  - The season bests of the raw drops dataframe above

3) Writes the first dataframe to excel for continuation of this project in R

4) Generates scatter plots and applies linear regression for the following parameters:
  - Every swim normalized by percent (NBP)
  - Comparison of Male and Female improvement NBP
  - Comparison of training group improvement NBP
  - Comparison of events by raw time drop
  - Comparison of each year's improvements NBP
  - Every season best NBP
 
5) Prepares a dataframe for feature analysis isolating features Sex, Training Group, Event, Percent Time Drop using career bests only

6) Changes the previous dataframe's categorical values into binary values

7) Uses sparse matrix feature analysis to see the contribution of each categorical value to the percent improvement

8) Clusters the data using KMeans and Principle Component Analysis to show the different groups of swimmers (i.e. Female Sprinter)
