# big-data-challenge


This project takes two large datasets from amazon's reviews, and performs ETL in google Colab, using RDS and Postgres SQL.

The first notebook reads in UK Data, and reduces it to several tables to match the required database schema; duplicates are dropped, cutomer ids grouped, etc.

The second notebook runs into a problem that I cannot get around, without combining the two notebooks (which the instructions say not to do). The 2nd notebook - despite coming from a separate country - features some customer ids that have already been put in from the first notebook. Since the database cannot have two of the same customer id, the import fails when it tries to bring these users in. To reiterate, I can see how this would be fixable by combining the data and grouping the customer ids before passing the data to SQL. 


