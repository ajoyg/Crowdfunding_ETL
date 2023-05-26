# Crowdfunding_ETL
ETL project 2 UCB Data Visualization Bootcamp
### Contributors: Ajay Gopalkrishna, Beethoven Sabar

The project builds an ETL pipeline using Python, Pandas, and regular expressions to extract and transform crowdfunding data (crowdfunding.xlsx and contacts.xlsx) from the Resources folder and creates clean datasets that includes campaign, category, subcategory, and contacts, the output is stored in 4 csv files with the same names in the Output folder.

The ETL_Mini_Project_final.ipynb Jupyter notebook does the following:
1. Reads the crowdfunding.xlsx file
2. Extracts the unique category and subcategory of funding and creates 2 csv files (Output/category.csv, Output/subcategory.csv)
3. Extracts and cleans the campaign data, merges it with the unique category and subcategory data and creates the campaign data in a csv file (Output/campaign.csv)
4. Reads the contacts.xlsx file
5. Separates the contact information into contact_id, first_name, last_name, and email
6. Creates the cleaned contacts data into a csv file (Output/contacts.csv)

The next step is to create the crowdfunding database from the above cleaned data.
1. Create the entity relationship (ER) diagram that shows the tables and their relationships between them. Refer to the Crowdfunding_db_ERD.png file.
3. Generate the DDL script to create the tables and constraits (Crowdfunding_db_DDL.sql)
2. Create the database in Postgres using PGAdmin, the name of the database is crowdfunding_db.  
3. Run the DDL script to create the tables
4. Import the csv data into the tables and add the table constraints
