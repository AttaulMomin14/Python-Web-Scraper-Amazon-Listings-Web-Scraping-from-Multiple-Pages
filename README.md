**Detailed Description**

In this Python project, I developed a web scraper to automate the extraction of product details from Amazon listings across multiple pages. The main tools used were the Beautiful Soup and Requests libraries, which facilitated the parsing of HTML content and HTTP requests.

**Steps Involved:**

**1- Importing Libraries:**
The necessary libraries were imported, including Beautiful Soup for parsing HTML, Requests for making HTTP requests, and Pandas and NumPy for data manipulation.

**2- Defining Functions:**
- Several custom functions were created to extract specific product details from the HTML content. These functions targeted various elements on the product page, including:
- get_title(soup): Extracts the product title.
- get_price(soup): Retrieves the product price, accounting for potential deals.
- get_rating(soup): Gathers the product's rating.
- get_review_count(soup): Counts the number of user reviews.
- get_availability(soup): Checks the product's availability status.

**3- Scraping Multiple Pages and Saving Data:**
- The script iterated through multiple Amazon listing pages, sending HTTP requests to each page and collecting links to individual product listings.
- For each product link, the script extracted the relevant details by invoking the previously defined functions.
- The extracted data was stored in a dictionary, which was later converted into a Pandas DataFrame for easy manipulation.
- The final DataFrame, containing all the scraped data, was cleaned by removing any empty rows.
- The clean dataset was then saved to a CSV file (amazon_data.csv), ready for analysis.

This web scraping project successfully automated the process of gathering product data from Amazon, providing a structured dataset that can be used for various analytical purposes, such as price comparison, trend analysis, or inventory management.
