# Web Scraper for Quotes.toscrape.com
A Python web scraper that extracts quotes, authors, and tags from [quotes.toscrape.com](https://quotes.toscrape.com/). It supports both static HTML scraping (using `requests` + `BeautifulSoup`) and dynamic JavaScript rendering (using `Playwright`).

📦 Features
✅ Dual Scraping Modes
- Static scraping (faster, for simple websites)
- Dynamic scraping (handles JavaScript-rendered content)

✅ Pagination Support

- Automatically follows "Next" buttons to scrape all pages

✅ Data Export
- Saves quotes in a structured CSV file

✅ Polite Scraping
- Respects time.sleep() to avoid overloading servers

✅ Error Handling
- Falls back to dynamic scraping if static scraping fails
