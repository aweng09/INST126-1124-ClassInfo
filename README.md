# Schedule of Information Science (INST) Classes

## Description
This is a program intended to visually represent information about the Information Science classes at the University of Maryland thus far. While there is a Schedule of Classes program that is similar on Testudo, the built-in platform, This Schedule of Information Science (INST) Classes will extend its goal and describe various characteristics students are generally interested in. As of November 25, 2020, these features include sorting and searching by: the course number, course name, average semester grade, pass rate, professor, professor rating, and format of learning. Furthermore, users will be able to save classes that fulfill their wanted criteria, and the program will print them out at the end.

## How It Works
The program has been written in Python. It will have four functions, as follows: 1) determine if the user would like to sort or search 2) sort by user-specified criteria 3) search by user-specified criteria 4) save user-specified classes. 

The sorting and searching occurs by using the pandas Python Data Analysis library. By storing relevant class information in a CSV file, we are then able to delineate which specific rows in a spreadsheet (each representing one course) fulfill the user's requested criteria. Sorting is enabled by the pandas function sort_values, which recreates a dataframe with rows ordered by integer from least to greatest or alphabetized (in descending order), depending on the requested column. Search is reliant on finding which rows include a specified term.

Saving classes occurs by appending their 'call value' (leftmost number in each row) to a list and then looping through the dataframe to print the reiterated rows. This will use .iloc.

## Updates
### November 21st
- Began project. Made test CSV file of a few fake courses. Detailed the four necessary functions. Started work on the "function_selecting" function. 
### November 23rd
- Finished the function_selecting and search_courses functions. Ran into issues comparing the CSV "average semester grades" and "pass rates" to the user input because we did not know they were recognized as integers instead of strings. Resolved by casting integer to user input.
### November 25th
- Began the sort_courses function. Began to collect relevant data necessary for actual implementation.

## Issues & Troubleshooting
- Running into issues with finding the relevant data; thus far, have decided to use PlanetTerp. Looking for ways to resolve any potential inaccuracies.

Please keep in mind that this program is reliant on matching user inputs to internal strings; if the program is malfunctioning, please consider typing your prompted answers exactly as they exist in the instructions. 

## Acknowledgements
As of November 25, 2020, we have used these following sources:
- PlanetTerp
- The pandas Python Data Analysis library
