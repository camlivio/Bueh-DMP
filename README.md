# Bueh-DMP
This Data Management Plan is based on [Eleanor Mattern's template (2022: 68)](https://direct.mit.edu/books/oa-edited-volume/5244/chapter/3537372/The-Linguistic-Data-Life-Cycle-Sustainability-of). 

## General Information 
	•	Title of the data set: bue_data 
	•	Camila Lívio, University of Georgia, camila.emidio25@uga.edu
	•	Chad Howe, University of Georgia, chowe@uga.edu
	•	Date of data collection: June of 2021
	•	Keywords describing the data topic: Twitter; digital-mediated communication; language of the internet; Angolan Portuguese
	•	The data set is in Angolan Portuguese, with variables titles in English 
	•	The collection of the data was not funded 

## Data File and Overview 
	•	The data was collected and processed using the R programming language 
	•	The data set contains structured data organized in columns and rows, consisting of numerical and categorical variables. 
	•	The file was saved in both .csv and .rds formats
	•	The file was created in 2021-06-21

## Sharing and Access Information 
	•	The data was collected via a Twitter Developer API account intended for research purposes. Currently, the Terms of Agreement of the social media platform have been updated, precluding us from publicly releasing the data set.
	•	Link to publication that cites the data: https://www.mdpi.com/2226-471X/9/3/82

## Methodological Information 
	•	The search string used to collect the data consisted of a list of high frequency adjectives in Portuguese (bom|boa, feliz, fixe, triste, especial).
	•	The data was collected and organized via Twitter's REST and stream Application Program Interfaces (API) through the package Rtweet (Kearney 2020) 
	•	The resulting data set is a data frame of 10,000 rows and 90 variables. 
	•	We checked the data for duplicates, cleaned it, and retained 9 variables of interest: user_id, created_at, screen_name, source, display_text_width, is_retweet, symbols, lang, quoted_location
	•	We removed Portuguese stop_words (Lopes 2013), and tokenized the text using the package Tidytext (Silge and Robinson 2016)
	•	The source code used to calculate the association strength between words was based on Schweinberger’s (2023) tutorial, and it can be found [here](https://ladal.edu.au/coll.html)

