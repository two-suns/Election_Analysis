# Election Analysis

## Project Overview
A Colorado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional election.

1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes each candidate received.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.

## Resources
- Data Source: election_results.csv
- Software: Python 3.10.1, Visual Studio Code, 1.63.2

## Summary
The analysis of the election show that:
- There were 369,711 votes cast in the election.
- The candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
- The candidate results were:
  - Charles Casper Stockham received 23.0% of the vote and 85,213 votes.
  - Diana Degette received 73.8% of the vote and 272,892 votes.
  - Raymon Anthony Doane received 3.1% of the vote and 11,606 votes.
- The winner of the election was:
  - Candidate Diana DeGette, who received 73.8% of the vote and 272,892 votes.

## Challenge Overview
### Purpose
The election commission has requested additional data to complete the audit.

1. The voter turnout for each county.
2. The percentage of votes from each county out of the total count.
3. The county with the highest turnout.

### Results
The further analysis of the data shows that:  
- Of the 369,711 total votes cast in the election,
  - The counties were:
    - Jefferson
    - Denver
    - Arapahoe
  - The county results were:
    - Jefferson received 10.5% of the vote and 38,855 votes.
    - Denver received 82.8% of the vote and 306,055 votes. 
    - Arapahoe received 6.7% of the vote and 24,801.
  - The county with the highest turnout was:
    - Denver, which received 82.8% of the vote and 306,055 votes.
## Challenge Summary
### Proposal
This script can be used for any election.  It may need to be modified to reflect the correct file path to the pertinent files on the user's computer.

<img width="548" alt="code_snip_path" src="https://user-images.githubusercontent.com/59906657/150364351-4a259b47-d31b-4372-a491-dea974258251.PNG">  

The os.path.join() method shown above can be updated to match the correct location of files on the user's computer.  Also, they can remove this method altogether and just input the full path depending on their preference. 

Also, if the percentages of the vote become too close, the amount of floating decimal places can be edited in the places indicated with arrows below. 

<img width="657" alt="code_snip_float" src="https://user-images.githubusercontent.com/59906657/150365730-b3011ab5-30b8-4841-a53d-44f146ede4db.PNG">  

The `.1f` can be modified to the necessary amount of decimal places to get a unique number in order to decide the election.

One other place the code may need to be modified is shown in the following image.  

<img width="512" alt="code_snip_row" src="https://user-images.githubusercontent.com/59906657/150368196-2d9596af-2134-4bca-acbe-37bf0414b2c5.PNG">  

Depending on the arrangement of the data in the resource file it is taken from, the row indexes may not match up exactly.  Updating the row selector in the brackets of the `row[]` section will assure the script is pulling the correct data.

Finally, with the above modifications, I believe this script is perfect to quickly and accurately get the results of any election that the commission conducts. 
