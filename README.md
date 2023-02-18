# Congress.gov Law Scraper

This is a Python script that scrapes all the laws from the website Congress.gov and saves them to an Excel file. The script uses the Selenium library to interact with the website and BeautifulSoup to parse the HTML.
Getting Started

To use this script, you will need to have Python 3 and the following libraries installed:
* Selenium
* BeautifulSoup
* pandas
* openpyxl
* webdriver_manager

You can install these libraries by running the following command in your terminal:

```python
pip install selenium beautifulsoup4 pandas openpyxl webdriver_manager
```

You will also need to have a web driver installed for your preferred browser.
This script has been tested with Firefox and its corresponding driver, GeckoDriver, but it should work with other browsers as well. 
Once you have downloaded the driver, make sure to add it to your system path.

### Running the Script

To run the script, simply navigate to the directory containing the script and, in your terminal, run:

`python law_scraper.py`

The script initializes the driver and creates a dataframe with two columns, namely title and description. Then, it saves each law to an Excel file named "law_names.xlsx" and outputs the number of titles found.

### Customizing the Script

If you want to change the starting URL or the number of pages to scrape, you can do so by editing the "BASE_URL" and "NUM_PAGES" variables at the top of the script. You will of course have to find new XML paths, etc. 

You can also customize the column names and order of the Excel file by editing the "columns" variable in the main() function.

### Contributing 

If you find any issues with this script or have suggestions for improvement, feel free to open an issue or submit a pull request. 
