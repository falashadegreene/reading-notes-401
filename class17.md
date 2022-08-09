# Web Scraping

## Web Scrape with Python in 4 minutes

1. Download data from the site
2. Check website terms and conditions and make sure not to download data too fast or it can crash website.
3. inspect website by finding where we can locate the links to files you want to download inside html tags. on the website, right click to inspect to view the raw code.

4. click on arrow and then click area of code to highlight in the console.
5. Start importing the following libraries:

`import requests
import urllib.request
import time
from bs4 import BeautifulSoup`

6. set the url to website and access the site with request libarary. if access works the ouput should show a #200 response.

7. then parse the html:

  `soup = BeautifulSoup(response.text, “html.parser”)`

8. use method .findAll to locate all of `<a>` tags

9. extract actual link

## What is Web Scraping?

Web scraping is a way to access and extract large amounts of data or information from a website. when web scrapping always read the websites terms and conditions to understand how to utilize the data legally. Make sure you are not downloading data too rapidly or it can cause the websit to crash. 

## How to scrape websites without getting blocked

- Check if websites is changing layouts
- Rotate user agents and corresponding HTTP Request Headers between requests
- Avoid scraping data behina a login
- Don't follow the same crawling patten

## Things I want to know more about 

what the specfic cases where we would use web scraping?