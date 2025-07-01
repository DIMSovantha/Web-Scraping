# Web Scraper for Quotes.toscrape.com
A Python web scraper that extracts quotes, authors, and tags from [quotes.toscrape.com](https://quotes.toscrape.com/). It supports both static HTML scraping (using `requests` + `BeautifulSoup`) and dynamic JavaScript rendering (using `Playwright`).

# 📦 Features
## ✅ Dual Scraping Modes
- Static scraping (faster, for simple websites)
- Dynamic scraping (handles JavaScript-rendered content)

## ✅ Pagination Support
- Automatically follows "Next" buttons to scrape all pages

## ✅ Data Export
- Saves quotes in a structured CSV & excel (.xlsx)file

## ✅ Polite Scraping
- Respects time.sleep() to avoid overloading servers

## ✅ Error Handling
- Falls back to dynamic scraping if static scraping fails

⚙️ Installation
1. Clone the Repository
```
git clone https://github.com/your-username/quotes-scraper.git
cd quotes-scraper
```
2. Install Dependencies
```
pip install requests beautifulsoup4 playwright
playwright install chromium
```
3. Run the Scraper
```
python scraper.py
```
(or run in Jupyter Notebook if using the .ipynb version)

# 📂 File Structure
```
quotes-scraper/
│── scraper.py            # Main Python script
│── quotes.csv            # Output file (generated after running)
│── README.md             # This file
└── requirements.txt      # Dependencies (optional)
```
(If using Jupyter Notebook, you may also have scraper.ipynb.)

# 📊 Sample Output (CSV)
```
text	                                |author	                  |tags
__________________________________________________________________________________________
"The world as we have..."	            |Albert Einstein	        |change,deep-thoughts...
"It is our choices..."	              |J.K. Rowling	            |abilities,choices
"There are only two ways..."          |Steve Jobs	              |inspirational,life
```

# 🚀 Possible Improvements
- Add async support for faster scraping (`httpx` + asyncio)
- Proxy rotation for large-scale scraping
- Logging for debugging
- CLI arguments for custom URLs/output files

# 🎯 Happy Scraping! 🚀

(Replace `your-username` with your actual GitHub username when cloning.)

# 🔗 How to Contribute
1. Fork the repo
2. Create a branch (`git checkout -b feature/new-feature`)
3. Commit changes (`git commit -m "Add new feature"`)
4. Push to branch (`git push origin feature/new-feature`)
5. Open a Pull Request

