![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Project: Data Cleaning and Manipulation with Pandas

## Overview


---

## Process
1 Import File into Jupyter Notebook + Google Tables 
    - Google Tables for easier visualization
    - Check columns
    - Go through each column, check values and look for cleaning potential

2 Check for missing values
    - Two unnamed columns without values
    - 'Time' with more than 50% of missing values 
    -> drop these columns
    
3 Column 'Country'
    - Not all entries are upper case -> change all to upper case
    
4 Column 'Name'
    - Column contains gender information which is already contained in column 'sex' -> empyt these values
    
5 Column 'Sex'
    - Column name contains a whitespace -> remove this white space
    - Values not consistent. Remove values with unclear information
    - Standardize clear information (e.g. 'M ' into 'M')
    
6 Column 'Age'
    - Column type obj and not standardized values
    --> Change column type into integer while dropping all values which are purely integer
    
7 Columns 'Href formula' & 'Href'
    - Column entires look identical --> Compare columns
    -> Columns are not identical: Some links in 'Href' are longer while containg twice the URL. Reason unknown. Keep columns.
    
8 Column 'Case Number'
    - 3x Times in data set -> drop last two columns
    
9 Convert into new csv

## Methods used

- Import CSV
- Identify missing values
- Drop columns
- Identify unique values
- Change column values into upper case
- Replace column entries
- Rename column name
- Change column data type
- Remove column values
- Compare two columns
- Convert to dataframe into csv

## Possible next steps
- Clean date with regex 



