## rightmove_scraper

This is a Python script for scraping property data from Rightmove and storing the results in a CSV file. It uses the `requests` library for making HTTP requests, and `BeautifulSoup` for parsing the HTML.

### Getting Started

1. Clone the repository or download the script.
2. Install the required libraries using pip: `pip install requests beautifulsoup4`
3. Open the script in a text editor and change the `location` variable to the desired location identifier.
4. Run the script: `python rightmove.scraper.py`

### Usage

The `RightmoveScraper` class has the following methods:

- `fetch(url)`: Makes an HTTP GET request to the specified URL and returns the response.
- `parse(html)`: Parses the HTML content using BeautifulSoup and extracts the property data.
- `to_csv()`: Writes the property data to a CSV file named "rightmove.csv".
- `run(location)`: Runs the scraper for the specified location identifier. The script will scrape data for the first five pages of property results and store them in a CSV file.

### Location Identifiers

Here are some example location identifiers for different cities in the UK:

- `REGION%5E1021`: London
- `REGION%5E1646`: Liverpool
- `REGION%5E902`: Bath
- `REGION%5E1050`: Birmingham
- `REGION%5E1429`: Bristol

To use the scraper for a different location, you can find the identifier by going to the Rightmove website and searching for properties in the desired location. The identifier will be included in the URL of the search results page.
