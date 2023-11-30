# NoSQL
MongoDB

## Instructions
The main aim of this challenge is to analyze data provided by he The UK Food Standards Agency. We have been tasked to evaluate some of the ratings data. The assignment is divided into three parts.

### Part 1: Database and Jupyter Notebook Set Up 
In the first part, I included the mongoimport command text used to import establishments.json in a markdown cell at the beginning of my Jupyter notebook file. The mongoimport command text correctly drops any existing establishments collection before importing establishments.json into MongoDB. The database is named uk_food and the collection is named establishments as required. 
In the next step, an instance of the Mongo Client is created and the database and collection name are reviewed.

### Part 2: Update the Database 
In the second part, I added an additional restaurant called "Penang Flavours" into the establishments collection. I started with a query which is performed to find the BusinessTypeID for "Restaurant/Cafe/Canteen" and returns only the BusinessTypeID and BusinessType fields.
The "Penang Flavours" document is updated with the correct value for BusinessTypeID.
Further, a query is correctly performed to delete all the documents in the collection where "Dover Local Authority" is the value for LocalAuthorityName. A count_documents() check is performed before and after the removal of the Dover documents to ensure the documents were removed. An update_many() query is performed to convert the latitude and longitude fields from strings to decimal numbers and RatingValue to integers.

### Part 3: Exploratory Analysis 
Four main questions needed to be answered for this part. 
Question 1: Which establishments have a hygiene score equal to 20?
Question 2: Which establishments in London have a RatingValue greater than or equal to 4? 
Question 3: What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
Question 4: How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas. 

Finally, I needed to submit a link to a GitHub repository that’s cloned to my local machine and contains my files.
I include appropriate commit messages in the files.


