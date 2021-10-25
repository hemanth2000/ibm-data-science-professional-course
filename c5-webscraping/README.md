# Web Scraping

Web scraping is a process of extracting information from a website using HTML tags. Manually collecting the essential data for a Data Science project is a cummbersome process. Web scraping tools comes in handy to gather information from websites.

Two modules, `Requests` and `BeautifulSoup` in python are used for web scraping in this project.

Sample code is shown below.

```python
import requests
from bs4 import BeautifulSoup

page=requests.get("https://www.WEBSITEURL.com").text

soup=BeautifulSoup(page,'html.parser') #parsing the html string using BeautifulSoup object

tag_object=soup.title # returns title tag of webpage

```
