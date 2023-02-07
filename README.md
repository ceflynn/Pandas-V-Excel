# Pandas Vs Spreadsheet

## Background

This notebook was created in response to an interview challenge to wrangle data using excel or google sheets.  The problem called for performing 3 tasks involving dealing with names, address and grades of students and their parents.  I completed the project with google sheets and submitted it as an excel file as requested.  After my submission, I realized that since learning pandas I had not used a spreadsheet to work with data, and how much easier it would have been to make a mistake or overlook something. So I decided to create a better way to address the problems presented in the challenge. 

I first created a solution with the same assumptions I had on the data when working in the spreadsheet.  I provided a slightly more sophisticated solution, but tried to make it as simple as possible.  

Then I tried to create a solution with some "less clean" data added to the dataset and this is where I discovered my error...

## Steps

* Split Guardian (Column B) and Scholar (Column E) names into separate First and Last
name Columns.
* Split Complete Address (Column D) into these separate Columns
    o Address (including unit numbers)
    o City
    o State
    o Zip
* Convert Scholar Grades (Column F) into this consistent format
    o Kindergarten
    o 1st
    o 2nd
## My Oversight 

I made the assumption that all of the names that need to be split had only a first and last name.  I was wrong! Somehow 'Chad Michael Murray' (famous actor name) did not catch my eye or cause any trouble when I was splitting text to columns in the spreadsheet.  