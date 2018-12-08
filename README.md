**Name**: Zhiming Huang  
**Online Demo**:  https://youtu.be/IlHRRdsn9xQ  
**Project Title**: Wordcount  
**Course**:  CCPS530 Fall 2018  
**Instructor**: Ghassem Tofighi  

## Wordcount app
A simple web app that calculates word-frequency pairs based on the text from a given URL

## Main languages/libraries used
Python, Flask, Flask-Migrate, Flask-Script, Flask-SQLAlchemy, PostgreSQL, BeautifulSoup, Natural Language Toolkit (NLTK), Bootstrap, JQuery

## How it works
The app takes an URL as input, reads the contents of the page and uses BeautifulSoup to 'clean' the text by removing the HTML tags, then it uses NLTK to 'tokenize' the raw text into individual words.  It then reads through the words and keep counts for each one, punctuation and words like 'I', 'me', 'the' are excluded from the count.  Lastly, it saves the results to the database and displays the results in a table (only the top 20 counts are displayed).  

## Watch the Video
![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/IlHRRdsn9xQ/0.jpg)  
(https://www.youtube.com/watch?v=IlHRRdsn9xQ)

## Deploy the app on Heroku
Follow the steps below to deploy it on Heroku (it's assumed that you are familiar with git and Heroku:

 1. Download the repo
 2. Create a new app on Heroku: *heroku create wordcount*
 3. Add the new app to git remote: *git remote add wordcount git@heroku.com:wordcount.git*
 4. Push code to Heroku: *git push wordcount master*
 5. Heroku should detect it's a Python app and deploy it
 6. Open the deployed URL to run it.
	
