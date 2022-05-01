# USAID-Scrapper

This project aims to scrape menu results, page link results and grants table entries from multiple USAID web pages. 

Example pages that can be scraped:

* For menu and page link results: https://www.usaid.gov/bangladesh
* For grants table results: https://www.grants.gov/web/grants/search-grants.html

### Code Files 
The repository contains the following code files :

* ```learn.py``` : Code to learn menu and page link scrapers
* ```fetch.py``` : Code to save last states for menu, page links and grant results
* ```compare.py``` : Code to compare current with last states for menu, page links and grant results, and store result difference
* ```utils.py``` : Utility functions
* ```config.py``` : Configuration file

### Steps To Run Code Files
* Run ```pip install requirements.txt```
* Run ```learn.py``` once to get learnt scrapers which are saved as ```learnt_scrapers.pkl```
* Run ```fetch.py``` once to get initial states which are saved as ```last_saved_links.pkl``` and ```last_saved_grants.pkl```
* Run ```compare.py``` to get result difference in current and last states which are saved as ```diff_links.json``` and ```diff_grants.txt```. This also updates the ```last_saved_links.pkl``` and ```last_saved_grants.pkl``` files with current results.
