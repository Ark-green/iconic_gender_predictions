# Background
most online shorppers only provide bare minimum of information needed when signing up as a new user or making a transaction on the site (i.e credit card details, delivery address etc). They do not provide their age, gender or any other personal details when they register as a new customer or they will simply purchase their items as a ‘Guest’ user.

## Solution Overview
* Transaction data: saved as a database file (test_data.db.zip) and a json file (test_data.json.zip). 
* steps in data preparations/processing:
    * Stage 1:
        1. unzipping the database file usig an encrypted password
        2. using sqlite 3 to connect to the database file (test_data.db)
        3. finding the table name within the database file (customers)
        4. writing SQL queries to answer stage 1 SQL questions on 'customers' table 
    * Stage 2 & 3:
        1. unzipping the json file, converting to a pandas dataframe for data preprocessing 
        2. creating new features for k-means unsupervised learning to predict gender (2 clusters)
    * Stage 4: documentation

## Tasks

### Stage 1: SQL 
 Using test_data.db to write SQL queries to answer the following questions:

* What was the total revenue ($) for customers who have paid by credit card?
* What % of customers who have purchased female items have paid by credit card?
* What was the average revenue for customers who used either iOS, Android or Desktop?
* To run an email campaign promoting a new mens luxury brand, list of customers to target?

### Stage 2: 
Data preprocessing and cleaning (two columns are intentionally corrupted, to be identified and fixed)

### Stage 3: 
BUILD - Building a model to predict the gender using the features provided and engineered 
* there is no gender flag --> unsupervised learning

### Stage 4: 
Documentating the process, findings and code into a reproducible document that can be understood by a business user and answers:
* How did you clean the data and what was wrong with it?
* What are the features you used as-is and which one did you engineer using the given ones? What do they mean in the real world?
* What does the output look like - how close is the accuracy of the prediction in light of data with labelled flags?
* What other features and variables can you think of, that can make this process more robust? Can you make a recommendation of top 5 features you'd seek to find apart from the ones given here
* Summarize your findings in an executive summary

* A repo of the code branch is available at:
