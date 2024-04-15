# Web-Scraping-using-Python


## Overview

The project web scraping using Python aims at Scraping the list of largest companies in india, according to 2021 fortune list from wikipedia website using Python and its libraries. It leverages popular libraries like BeautifulSoup and requests to scrape web pages and extract the desired information.

## Operations performed

- **Data Extraction**: Extract specific data elements from wikipedia websites.
- **Customization**: Easily customizable for scraping different websites or different data points.
- **Scalability**: Can handle scraping large volumes of data efficiently.
- **Error Handling**: Includes robust error handling to handle various scenarios encountered during scraping.

## Prerequisites

Before running the scraper, ensure you have the following installed and imported:

- Python: Install jupyter notebook from [jupyter.org](https://jupyter.org/)
- BeautifulSoup: Import using `bs4 install beautifulsoup`
- Requests: Import using `import requests`

## Installation

Install the required dependencies:

```bash
from bs4 import BeautifulSoup
import requests
```

## Usage

1. Modify the `config.py` file to specify the URLs and data points you want to scrape.
2. Run the scraper using the following command:

```bash
url = 'https://en.wikipedia.org/wiki/List_of_largest_companies_in_India'

page = requests.get(url)

Soup = BeautifulSoup(page.text, 'html')
```

3. The scraped data will be saved in [Companies.csv].

## Examples

Below are some examples of how to use code to form table:

```python
for row in column_data[1:]:
    row_data = row.find_all('td')
    individual_row_data = [data.text.strip() for data in row_data]
    
    
    length = len(df)
    df.loc[length] = individual_row_data
```

## Contributing

Contributions are welcome! If you have any ideas for improvement or want to fix a bug, feel free to submit a pull request.


## Acknowledgments

- The [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) library for its powerful HTML parsing capabilities.
- The [Requests](https://docs.python-requests.org/en/latest/) library for simplifying HTTP requests in Python.

---

