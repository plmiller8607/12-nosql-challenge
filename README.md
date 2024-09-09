# 12-nosql-challenge
Evaluation of Restaurants in the UK using MongoDB

# Overview 

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. This project involves evaluating some of this ratings data for the editors of a food magazine, Eat Safe, Love in order to help their journalists and food critics decide where to focus future articles. The project is divided into three parts: Part one involves Database and Jupyter Notebook setup; Part two requires updating the database; and Part three is an exploratory analysis of the results.

# Resources 
Jupyter notebook files
Json file



# Usage 
Import the data provided in the establishments.json file with the code: "mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json"
Name the database “uk_food” and the collection “establishments”
Update the database by adding new restaurant called "Penang Flavours"
Remove restaurants located in Dover
Perform exploratory analysis to answer the following questions:
1. Which establishments have a hygiene score equal to 20?
2. Which establishments in London have a RatingValue greater than or equal to 4?
3. What are the top 5 establishments with a RatingValue rating value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establishments in each Local Authority area have a hygiene score of 0?
For each question Use “count_documents” to display the number of documents contained in the result.
Display the first document in the results using pprint. Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.




# Dependencies
from pymongo import MongoClient
import pandas as pd
from pprint import pprint



# License
This project is licensed under the MIT License - see the LICENSE file for details.
