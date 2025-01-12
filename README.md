
# Book Store Web Scraper

This project is a web scraper designed to extract book information from [Books to Scrape](https://books.toscrape.com/). The script retrieves details such as the title, price, rating, stock availability, and URL for each book listed on the site. The scraped data is saved into an Excel file for further analysis.

## Features

- Scrapes book information from up to 50 pages of the website.
- Extracted data includes:
  - **Title**: The name of the book.
  - **Price**: The price of the book.
  - **Rating**: The book's rating (e.g., One, Two, Three stars, etc.).
  - **Stock Availability**: Whether the book is in stock or not.
  - **URL**: A direct link to the book's details page.
- Saves the scraped data into an Excel file (`books.toscrape.xlsx`).

## Technologies Used

- **Python**: For writing the script.
- **BeautifulSoup**: For parsing the HTML content.
- **Requests**: For making HTTP requests to the website.
- **Pandas**: For data manipulation and exporting to Excel.

## How It Works

1. **Request Pages**: The script sends requests to the website, iterating through multiple pages to scrape data.
2. **Parse HTML**: It uses BeautifulSoup to parse the HTML structure and locate book details.
3. **Extract Data**: Extracts the title, price, rating, stock availability, and URL for each book.
4. **Save Data**: Stores the extracted data in a structured format and exports it as an Excel file.

## Example Output

| Index | Title                       | Price   | Rating   | Stock Availability | URL                                        |
|-------|-----------------------------|---------|----------|--------------------|--------------------------------------------|
| 1     | A Light in the Attic       | £51.77  | Three    | In stock           | https://books.toscrape.com/...            |
| 2     | Tipping the Velvet         | £53.74  | One      | In stock           | https://books.toscrape.com/...            |

## Notes

- Ensure that the website allows scraping by checking its terms of service.

## Contribution

Feel free to fork the repository and submit pull requests for improvements or bug fixes.
