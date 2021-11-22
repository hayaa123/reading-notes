# Web scraping

- also called web harvesting, or web data extraction

-  is data scraping used for extracting data from websites.

## How to Web Scrape with Python

1- Find the URL that you want to scrape.
2- Inspecting the Page.
3- Find the data you want to extract.
4- Write the code.
5- Run the code and extract the data.
6- Store the data in the required format.

First, let us import all the necessary libraries:

```python 
from selenium import webdriver
from BeautifulSoup import BeautifulSoup
import pandas as pd
```
To configure webdriver to use Chrome browser, we have to set the path to chromedriver

```python 
driver = webdriver.Chrome("/usr/lib/chromium-browser/chromedriver")
```

Refer the below code to open the URL:

```python 
products=[] #List to store name of the product
prices=[] #List to store price of the product
ratings=[] #List to store rating of the product
driver.get("<a href="https://www.flipkart.com/laptops/">https://www.flipkart.com/laptops/</a>~buyback-guarantee-on-laptops-/pr?sid=6bo%2Cb5g&amp;amp;amp;amp;amp;amp;amp;amp;amp;uniq")

```

it’s time to extract the data from the website

```python
content = driver.page_source
soup = BeautifulSoup(content)
for a in soup.findAll('a',href=True, attrs={'class':'_31qSD5'}):
name=a.find('div', attrs={'class':'_3wU53n'})
price=a.find('div', attrs={'class':'_1vC4OE _2rQ-NK'})
rating=a.find('div', attrs={'class':'hGSR34 _2beYZw'})
products.append(name.text)
prices.append(price.text)
ratings.append(rating.text) 
```

Run the code `python web-s.py`

## Is Web Scraping Legal?
you can look at the website’s “robots.txt” file. You can find this file by appending “/robots.txt” to the URL that you want to scrape.

https://www.edureka.co/blog/web-scraping-with-python/