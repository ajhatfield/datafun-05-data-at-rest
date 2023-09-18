# Files, Exceptions, and SQL

- [GitHub Repository](https://github.com/ajhatfield/datafun-05-data-at-rest)

In this assignment, you'll read from data files, process the data, and write to output files. We'll also look at using Python to work with light-weight, file-based relational database SQLite using the sqlite3 module from the Python Standard Library. 

Chapters: Work through the book and examples from Chapters 9 and 17.2 (SQL).

## Task 1 - Read and work through Chapter 9 - Files & Exceptions - understand the examples. 

9.1 Introduction
9.2 Files
9.3 Text-File Processing
    9.3.1 Writing to a Text File: Introducing the with Statement
    9.3.2 Reading Data from a Text File
9.4 Updating Text Files
9.5 Serialization with JSON
9.6 Focus on Security: pickle Serialization and Deserialization
9.7 Additional Notes Regarding Files
9.8 Handling Exceptions
    9.8.1 Division by Zero and Invalid Input
    9.8.2 try Statements
    9.8.3 Catching Multiple Exceptions in One except Clause
    9.8.4 What Exceptions Does a Function or Method Raise?
    9.8.5 What Code Should Be Placed in a try Suite?
9.9 finally Clause
9.10 Explicitly Raising an Exception
9.11 (Optional) Stack Unwinding and Tracebacks
9.12 Intro to Data Science: Working with CSV Files
    9.12.1 Python Standard Library Module csv
    9.12.2 Reading CSV Files into Pandas DataFrames
    9.12.3 Reading the Titanic Disaster Dataset
    9.12.4 Simple Data Analysis with the Titanic Disaster Dataset
    9.12.5 Passenger Age Histogram

## Task 2 - Read and work through Chapter 17 - Big Data - understand the examples. 

17.1 Introduction
17.2 Relational Databases and Structured Query Language (SQL)
    17.2.1 A books Database
    17.2.2 SELECT Queries
    17.2.3 WHERE Clause
    17.2.4 ORDER BY Clause
    17.2.5 Merging Data from Multiple Tables: INNER JOIN
    17.2.6 INSERT INTO Statement
    17.2.7 UPDATE Statement
    17.2.8 DELETE FROM Statement

## Task 3 - Titanic Passengers (from 9.12 above)

1. Follow the instructions in 9.12.3 (starting pg. 346).
2. Don't work in interactive mode!
3. Instead complete the exercise in a Jupyter notebook. 
4. Perform the following subtasks.
5. Required: Include the title of the notebook, and your name and date at the top.
6. Required: Use Section headings in your Markdown to make it clear that each of these 6 sections are shown in your notebook. They should be numbered 1-6 and include the keyword shown below.
7. Recommended: Use titles and section headings in every notebook. Communication is important and clear organization is valuable.
8. Section 1-Load: Use pandas to read in the Titanic Disaster dataset csv file.
9. Section 2-View: Set the precision to 2 decimal places. View the head and tail of the file.
10. Section 3-Headings: customize the column headings.
11. Section 4-Describe: Use the DataFrame describe() function to calculate basic descriptive statistics for all numeric columns. 
12. Section 5-Survivors: Follow instructions to describe statistics for those who survived (titanic.survived == 'yes') - see the example. 
13. Section 6-Histogram: Use the DataFrame's hist() function to create a histogram for each numerical column.

Helpful Hints:

1. Notice that describe() provides different results for non-numeric data (e.g., unique, top, freq)
2. Enable matplotlib. If it doesn't work (e.g., in a notebook), try 
    %matplotlib inline

Output: 

Document your results.
execute the completed notebook before you commit and push to GitHub

## Task 4 - SQL (from 17.2 above)

1. Follow the instructions in 17.2.1 (starting pg 730) 
2. Don't work in interactive mode - use a notebook.
3. IMPORTANT: create the table using the books.sql script provided with the author files. 
    1. If Windows, use Anaconda Prompt (generally for all commands we use in this course).
    2. Try to populate your own database from the script. If you can't, download a populated books.db Download books.db.
4. In your Python code, import the sqlite3 module and use the connect function to create a connection to your database.
5. After running the script, there should be 3 tables: authors, author_ISBN, and titles. 
6. Import pandas as pd
7. Use pd options.display to set the max_columns to 10
8. Use pd read_sql fuction to select everything (*) from the authors table, then the titles table, then the author_ISBN table.
9. Section 1: SELECT. Complete 17.2.2 SELECT (1 query)
10. Section 2: WHERE. Complete 17.2.3 WHERE (3 queries)
11. Section 3: ORDER BY. Complete 17.2.4 ORDER BY (4 queries)
12. Section 4: INNER JOIN. Complete 17.2.5 INNER JOIN (1 query)
13. Section 5: INSERT INTO. Complete 17.2.6 INSERT INTO (2 queries)
14. Section 6: UPDATE. Complete 17.2.7 UPDATE (2 queries)
15. Section 7: DELETE FROM. Complete 17.2.8 DELETE FROM (2 queries)
16. Section 8: SELECT. Show your Final Results, SELECT * from each table and display the final state of each of the 3 tables.
17. Required: Include the title of the notebook, and your name and date at the top.
18. Required: Use Section headings in your Markdown to make it clear that each of these 8 sections are shown in your notebook. They should be numbered 1-8 and include the SQL keyword shown above. Use a heading before your the final results showing all 3 tables as well. 

Output: 

Document your results.
execute the completed notebook before you commit and push to GitHub

## Task 5 - Push Repo to GitHub

Use VS Code to commit and sync (push) your repo to GitHub.

## Optional Task 6. Bonus

1. Start a new notebook.
2. Locate a unique csv dataset. 
3. Use pandas to import the csv dataset into a DataFrame.
4. Use the DataFrame commands to clean the data as needed and/or rename the columns.
5. Use the DataFrame describe() function to calculate basic descriptive statistics. 
6. Use the DataFrame hist() function to generate histograms for all numeric columns. 
7. Include the required heading at the top, and use section headings to tell your story with data. 
8. Execute the entire, professionally presented file and output to html. 
9. Git add, git commit, and git push the new content to your GitHub repo.

## Reflection (on your own)

1. What kinds of data at rest are available in your domain?
2. What kinds of data in motion are available in your domain? 
3. How important is it for a data analyst to be able to describe their data?  Do a web search for all that can be included.
4. Scan Kaggle to see how their datasets are described. 
