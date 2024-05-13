# WebScrapping
Scrapping or websites like amazon and aabtak news

# amazon:
Project Overview

o Imagine you're on a mission to learn all about what's being sold on Amazon, the giant online store.
You want to gather detailed info about the products (under the ‘Fashion’ Category only). They
offer so you can understand what people are buying and what's popular.
o To do this, you need to use a technique called web scraping, which means collecting data from
websites. But there's a catch – you have to follow Amazon's rules about how you can use their data.
o Your goal is to create a big collection of product information in a format called JSON. This format
is easy for computers to understand and work with, so it's great for analyzing data.
o Each piece of info about a product, like its name, price, and description, is neatly organized in this
JSON format. Once you've gathered all this data, you can study it to see what kinds of things people
are interested in buying on Amazon.

➢ You have to scrap at least 1000 products from each category. By category, it meant
i.e. shoes, clothes, watches, etc.

1. Data Preprocessing and Cleaning
Review and preprocess the collected JSON data to ensure quality and consistency. Focus on handling
missing values, standardizing text data (such as product descriptions and reviews), and formatting
numeric data appropriately.
For Example
• Identify and remove duplicates, and perform data type conversions as necessary for numeric
fields and dates (Only use Numpy, Pandas, and Matplotlib)
• Use natural language processing (NLP) techniques to clean and standardize reviews. This may
include removing stop words, stemming, and lemmatization. (use NLTK)
2. Image Data Handling
• Develop a strategy to download and store product images from the URLs collected in
Assignment 1. Consider storage efficiency and retrieval performance. (BONUS)
• Create a mechanism to link each image (in the form of a link) with its corresponding product
in the database.
3. Database Schema Design

• Design a relational database schema that includes tables. Ensure that each table is normalized
to reduce redundancy and improve data integrity.
• Include foreign keys in your schema to establish relationships between tables. This linkage is
critical for maintaining data consistency and supporting efficient queries.
4. Data Insertion and Querying
Write a Python script to insert the cleaned data into your database(MYSQL) according to the schema
you designed. Pay special attention to the handling of images, which may require storing paths to
image files.

#--------------------------------------------------------------------------------------------------------------------
#news channel:

Task Description:
1. Proxy IP Setup:
a. Obtain a list of proxy IPs. You can use free proxies for this task, but ensure they are from
a reliable source and are functional.
b. Implement a mechanism to rotate through these proxies with each request. Consider
using a Python library that supports proxy rotation or implementing a custom rotation
logic.

2. Scraping Multiple News Websites:
a. Select at least three news websites to scrape.
b. Write functions to send requests to these websites, rotating the IP address (proxy) with
each request to avoid IP bans.
c. Parse the HTML content of each website to extract news headlines and their publication
dates. The parsing logic will be unique for each website due to different HTML
structures.
3. Data Handling:
a. Structure the extracted data in a uniform format, e.g., a Python dictionary or directly
into a pandas DataFrame.
b. Save the scraped data into a CSV file, ensuring each entry contains the headline, source,
and publication date.

