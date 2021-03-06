# Election_Analysis

## Overview

This election audit was performed for a recent Colorado congressional election using Python and Visual Studio Code. The votes, which had been compiled into a csv file, were tallied and the following summaries were output into a txt file for the election commission: total votes, votes and percentage of votes by county, the county that had the highest voter turnout, votes and percentage of votes by candidate, along with a section calling out the election winner and their respective votes and vote percentage.

## Results

- ### Total Votes:

&nbsp; &nbsp; &nbsp; &nbsp; ![Total_Votes](https://user-images.githubusercontent.com/90863226/136712442-cf7f4ce2-1b1b-4519-a44e-58c4718b9c79.png)

- ### Votes by County:
 
 &nbsp; &nbsp; &nbsp; &nbsp; ![Votes_By_County](https://user-images.githubusercontent.com/90863226/136712095-53e8f3ee-abc4-4178-b2aa-d77c3b48f316.png)

- ### County with the highest voter turnout:

&nbsp; &nbsp; &nbsp; &nbsp; ![Largest_County](https://user-images.githubusercontent.com/90863226/136712457-146b455e-bef6-42df-afe7-5186048c4410.png)

- ### Votes by Candidate:

&nbsp; &nbsp; &nbsp; &nbsp; ![Votes_By_Candidate](https://user-images.githubusercontent.com/90863226/136712400-96185e26-b496-4c85-ac2f-75b77ac4be61.png)

- ### Election Winner:

&nbsp; &nbsp; &nbsp; &nbsp; ![Election_Winner](https://user-images.githubusercontent.com/90863226/136712271-dbe1ed54-bda5-4824-950c-f77bedec3ba8.png)

## Summary

This Python script was a quick and easy way to perform this election audit, and with a few minor modifications could be used to audit nearly any election. As long as the election votes are compiled in a csv file in a similar format you should be able to use this same code making the following modifications:

1. The file location, in row 9, for the file containing the compiled votes: `file_to_load = os.path.join("Resources", "election_results.csv")`
2. The file location, in row 11, where you would like to save the results: `file_to_save = os.path.join("analysis", "election_analysis.txt")`
3. Check to make sure the columns are in the same order and if not modify the following two lines of code:
   - row 48: `candidate_name = row[2]`
   - row 51: `county_name = row[1]`
