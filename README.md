# Web Scraping 
This project is to build a web application that scrapes various websites for data related to the Mission to Mars and displays the information in a single HTML page.
<hr>
## Initial scraping was done with Jupyter Notebook using following libraries:
**BeautifulSoup**
<br>
it is a Python library for pulling data out of HTML and XML files. It works with any parser to provide idiomatic ways of navigating, searching, and modifying the parse tree.
<br>
**Pandas**
<br>
this python's data analysis library can be used with BeautifulSoup for web scraping. BeautifulSoup can pass the findings to pandas. Pandas can use its read_html function to read the HTML table data into a dataframe, which can be converted to JSON format.
<br>
**Requests**
<br>
it is a Python library that is used to send HTTP requests, add headers, form data, multiplart files and parameters with simple Python dictionaries, and access the response data in the same way.
<br>
**Splinter**
<br>
it is an open source tool for testing web applications using Python. it lets you automate browser actions, such as visting URLs and interacting with their items.
<br>
## Defined a function to perform all the scraping:
* In a file scrape_mars.py, **scrape()** function was defined to execute all of the scraping code and return one Python dictionary containing all of the scrapped data.
<br>
## Flask and PyMongo
* Using Flask, created a route **(/scrape)** that imports the scrape_mars.py script and call the **scrape** function.
* Using PyMongo stored the return value in Mongo as a Python dictionary.
* Created a route **(/)** that queries the mongo database and passes the mars data into an HTML template to display the data
<br>
## HTML, CSS, Bootstrap
* Created an index.html file that takes mars data dictionary and displays all the data in appropriate HTML elements.

## Snapshot of the webpage
![Alt text](webpage.png?raw=true "Optional Title")
