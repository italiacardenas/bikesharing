# NYC Citi Bike Sharing Data Analysis using Tableau 
[link to dashboard](https://public.tableau.com/app/profile/italia.i.cardenas/viz/WhoisusingNYCCitibike/WhoisusingNYCCitibikeandwhenandwhere)

## Overview of the Bikesharing Analysis
This Bikesharing analysis was created to propose to potential investors a successful bikesharing system in Des Moines. 

Tableau, Jupyter Notebook, and Pandas were used to create this analysis. 

## NYC Bike-Sharing Results 
1. NYC Citibikes are mostly being used between 8am-9am and 5pm-7pm.
![AugustNYCuse.png](https://github.com/italiacardenas/bikesharing/blob/96251f32b64b3c1bc27f6e83b89e069ed386a22d/AugustNYCuse.png)

## Election Audit Summary
 In order to reproduce this script for any election with some modications the folllowing would be required:
 - VS Code
 - CSV file with elections result tabular data
 - Python 3.7.6
 
 1. The first steps require importing the csv and creating variables that will be used in *for loops* and *if statements* and setting them to zero such as, total votes, winning candidate's count, winning candidate's percentage, largest county turnout, and largest county percentage as well as empty string variables for winning candidate and largest turnout county.
 2. After setting the variables, two empty list must be created one for the different candidates and another for the different counties. Afterwords two empty dictionaries will be created, one to store the candidate votes count and another to store the vote counts by county.
 3. The location of the files that is loaded to use for the audit and the location of the text file that will be used to print the results will differ and therefore need to be modifed. In this example the *election_results.csv* file is in the **Resources** folder and the *election_analysis.txt* file is in the **analysis**, but for a different audit, it is important to modfy the code to the correct location. 
![file_locations.png](https://github.com/italiacardenas/Election_Analysis/blob/3f9895f6141a543a46a6a82b662f459dc3c0da89/Resources/file_locations.png)
4. The code must be modified to reflect the data in the csv file being used for the audit. In this case, candidate_name = row[2] and county_name = row[1] tells Python that the candidate names are in row 2 of the csv file and county names are in row 1. The data may be different in a different audit and the code must be modified.
![rows_referred_from_csv.png](https://github.com/italiacardenas/Election_Analysis/blob/3f9895f6141a543a46a6a82b662f459dc3c0da89/Resources/rows_referred_from_csv.png)   
 
