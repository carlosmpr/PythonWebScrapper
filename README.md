#  Simple Quote Web Scrapper 

Web Scraping with Python and Beautiful Soup and parse the quotes to a file

## Steps
1. Send an HTTP request to the URL of the webpage  to access. 
2. Once we have accessed the HTML content, we parse the data.
3. Navigating and searching the parse tree that we created, i.e. tree traversal

## Python packages to install
- pip install requests
- pip install html5lib
- pip install bs4

## Code 

1. Imports:
        
        import requests
        from bs4 import BeautifulSoup
        import csv
2. url:

        URL = "['Your webside']"
3. Making the request to the website:
     
        r = requests.get(URL)
4. Parse the result with beautiful soup:
        
        soup = BeautifulSoup(r.content, 'html5lib')
5. Print the result

        print(soup.prettify())
        