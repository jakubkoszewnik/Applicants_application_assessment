# Applicants Application Assessment

<img src="https://github.com/jakubkoszewnik/jakubkoszewnik/blob/main/data-cleaning.png" width="300">

This is an application assessment project :)

Libraries used in this project:
- Numpy
- Pandas

* First, I successfully imported CSV files.
* Then I cleaned the data by:
  - Removing duplicates,
  - Changing "NA" values in the "External Rating" column to 0,
  - Changing "NA" values in the "Education Value" column to "Average".

<img src="https://github.com/jakubkoszewnik/jakubkoszewnik/blob/main/score.png" width="300">

Next, the scoring criteria are as follows:
- The score should be a number from 0 to 100.
- The score is the sum of points awarded to the application based on 6 criteria.
- The score is zero if there is no 'Amount' value or if 'External Rating' is zero.
- Components of the score:
  - If the candidate's age is between 35 and 55 years old, add 20 points to the score.
  - If the application was submitted during the week, excluding the weekend, add 20 points to the score.
  - If the candidate is married, add 20 points to the score.
  - If the candidate lives in Warsaw or the Masovian Voivodeship, add 10 points to the score.
  - The 'Score' from the industries.csv table is also added to the score (ranging from 0 to 20 points).
  - If the 'External Rating' value is greater than or equal to 7, add 20 points to the score.
  - If the 'External Rating' value is less than or equal to 2, subtract 20 points from the score.
