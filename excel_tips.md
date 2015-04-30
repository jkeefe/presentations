# Excel Tips for Journalists

Presented at WNYC in April 2015. 

This document shortlinked at bit.ly/jk-excel-tips

# Quick Concepts

These are the things you can do when you first want to get to know your data

(Data sets using are School Vaccinations and Claims, which are not in this repo)

- Sort it a lot

- Check out the row count 
  - Does it pass the smell test?
  - Is it **65,536**?!? That is [bad](http://superuser.com/questions/366468/what-is-the-maximum-allowed-rows-in-a-microsoft-excel-xls-or-xlsx)!

- Do you know what the columns really mean?

  
- Look for things you think should be there (and whether they make sense)


# Math

(Data sets using are marijuana arrests, which are not in this repo)

- Using the Equals sign
  * Tells Excel "The rest is a formula"

- Sums

  - `=SUM(A1:A5)`
  - Can Drag to fill out the colums
  - Can just highlight cells for a quick preview at the bottom
  - Clicking on a formula cell shows you the boxes it's using

- Percentages 

  - (part divided by whole)
  - test: 10/100

- Percent Change

  - (New minus old) over old
  - (New - Old) / old
  - Parentheses matters!
    - Excel uses math precidence
    - AKA "Order of Operations"
    - Please Excuse My Dear Aunt Sally
    - Parens, Exponents, Multiplcation, Division, Addition, Subtraction
    - Percent change from 10 to 8?
      * 10 - 8 / 8 evaluates to **9** (10 minus 1) *wrong*
      * (10 - 8) / 8 evaulates to **.25** *right!*
  
- Numbers all the way down
  * Copy formulas down by starting with the original
  * Dragging the highlighting box down
  * Hitting `Ctrl-D`
  * (can also do this to the right, using `ctrl-R`)

- Changing column format
  * Click top of colum (the letter)
  * `Format` and then `Cells...`
  * Pick the format you want for the column


## Raw Records

When you have raw records -- one item per row -- you really need to be able to summarize!

(Using dogs data, not in this repo)

Pivot tables are how to do that. 

- Select entire data set using `ctrl-A`
- In menu, pick `Data` and then `Pivot table`
- Choose the column you'd like to see a summary of (like breed) and make it a ROW LABEL
- Choose the column you'd like to count (like, breed again!) and make it a ROW VALUE
- This will give you a count of those items
- For numerical values, you can also sum and average the values instead
- To sort the numerical value, put the cursor in the first box of actual data (!?!?!)
- From Menu, choose `Data` and then `Sort` ... and pick ascending or decending

Using Dogs data ...

- By dog breed (citywide)
- By dog name (citywide)
- By Boro, dog name
  * Do this by adding both Borough and Dog Name to the row labels

Use Claims data to show the summing



