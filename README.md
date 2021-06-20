# NYC Citi Bike Sharing Data Analysis using Tableau 
[link to dashboard](https://public.tableau.com/app/profile/italia.i.cardenas/viz/WhoisusingNYCCitibike/WhoisusingNYCCitibikeandwhenandwhere)

## Overview of Election Audit
This is an election audit of tabulated results completed by the Colorado Board of Elections for the U.S. Congressional Precinct in Colorado. The purpose of this election audit is to generate a vote count report to certify this U.S. Congressional race. The three voting methods taken into account were mail-in ballots, punch cards, and direct recording electronic. The report contains the total number of votes cast, the total number of votes for each candidate, the percentage of votes for each candidate, the winner of the election based on popular vote. 

The process was automated with Python 3.7.6. The automation was successful and may be used to audit other congressional districts, senatorial districts and local elections.

## Election-Audit Results 
- Total Votes Cast in this Congressional Election: **369,711**
- Number of Votes and Percentage of Total Votes by County:
  1. **Denver**    **|**    306,055  **|**  *82.8%*
  2. **Jefferson** **|**    38,855   **|**  *10.5%*
  3. **Arapahoe**  **|**    24,801   **|**  *6.7%*
- County with Largest number of votes: **_Denver_**
- Number of Votes and Percentage of Total Votes by Candidate:
  1. **Diana DeGette**             272,892   **|**  *73.8%*
  2. **Charles Casper Stockham**   85,213    **|**  *23.0%*
  3. **Raymon Anthony Doane**      11,606    **|**  *3.1%*
- Winner of the Election: **Diana DeGette**  Vote Count: **272,892**  Percentage of Total Votes: **73.8%**
  
![Screen Shot 2021-04-04 at 3.02.13 PM.png](https://github.com/italiacardenas/Election_Analysis/blob/3f2bd45ef045796f178a022020939c3cda357db3/Resources/Screen%20Shot%202021-04-04%20at%203.02.13%20PM.png)

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
 
