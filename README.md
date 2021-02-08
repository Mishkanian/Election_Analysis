# Election Audit and Analysis

## Project Overview
The purpose of this election audit and analysis is to determine the winner of an elction based on over 369,000 voter data points. Other objectives include determining total votes by County and the largest County turnout.
---

## Resources
**Data Source:** election_results.csv (found in "Resources")  
**Software:** Python 3.8.2

## Summary of Findings
The analysis of this election has shown the following results:
- There were **369,711 votes** in this election.
- Breakdown of total votes by County:
  - Denver has 306,055 votes (82.8% of the total votes).
  - Jefferson has 38,855 votes (10.5% of the total votes).
  - Arapahoe has 24,801 votes (6.7% of the total votes).
- **Denver County has the largest number of votes from a single County.**

- Breakdown of total votes by candidate:
  - Diana DeGette has 272,892 votes (73.8% of the total votes).
  - Charles Casper Stockham has 85,213 votes (23.0% of the total votes).
  - Raymon Anthony Doane has 11,606 votes (3.1% of the total votes).
- **The winner of the election is Diana DeGette.**
  - Diana DeGette received the most votes (272,892 votes).

## Project Challenges

## How to Modify Script for Future Elections
Modifying this script for future elections can be accomplished with the following methods:

The first step is changing the folder and file names on lines 9 and 11 of PyPoll to match your new data file names.
```python
9  file_to_load = os.path.join("Folder_with_data", "new_election_data.csv")
11 file_to_save = os.path.join("Folde_with_text_file", "new_analysis.txt")
```
It is important to inspect new CSV data files to determine the layout and location of data. On lines 47 and 50, your row indexes may need adjusting depending on the layout of your new data file:
```python
47 candidate_name = row[row_number_ with_candidate_here]
50 county_name = row[row_number_ with_county_here]
```
Author: Michael Mishkanian
