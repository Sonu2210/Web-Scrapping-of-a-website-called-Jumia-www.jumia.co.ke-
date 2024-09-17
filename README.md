Jumia Website Web Scraper (www.jumia.co.ke)
This project is a Python-based web scraper designed to extract product information (such as name, price, and rating) from the Jumia Kenya website using the BeautifulSoup library.

Table of Contents: 
  * Introduction
  * Prerequisite
  * Code Breakdown

* Introduction
  The Jumia Web Scraper retrieves product data from the Jumia Kenya website. It loops through the first 50 pages of all products, extracting product names, prices, and ratings.

* Prerequisites
  Before running the scraper, ensure you have the following installed:
    Python 3.x
    Required Python libraries:
    - requests
    - beautifulsoup4
    - pandas

* Code Breakdown
  Here is an overview of how the code works:
  Requests and BeautifulSoup: The requests.get() function fetches the HTML content from the Jumia website. BeautifulSoup is used to parse the HTML and extract the required information.

  Pagination: The script loops through the first 50 pages of Jumia products using a for-loop and appends the page number to the URL.

  Product Extraction: For each page, the script looks for product details using find_all() and extracts:
  - Name: Product name
  - Price: Product price.
  - Rating: Product rating, if available. If not, it defaults to 'None'.
  - Error Handling: If a product does not have a rating, the script will handle the exception and assign 'None' to the rating.
 
  
