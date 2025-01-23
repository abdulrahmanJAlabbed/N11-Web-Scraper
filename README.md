# N11 Web Scraper

A comprehensive web scraper for the N11 website built with Puppeteer. This script extracts product details, categories, and pricing information, and exports the data to a CSV file.

## ✨ Features
- Extracts category and product details from the N11 website.
- Handles infinite scrolling for dynamic content loading.
- Implements random delays for human-like behavior.
- Saves data in a structured CSV format.

## 📋 Prerequisites
- **Node.js** (>= 16.0.0)
- **Google Chrome** or **Chromium** installed on your machine.
- Basic knowledge of JavaScript and Puppeteer.

## 📦 Installation

1. Clone the repository:
```bash
   git clone https://github.com/yourusername/n11-web-scraper.git
   cd n11-web-scraper
```
2.Install dependencies:
```bash
npm install puppeteer fast-csv
```

🚀 Usage
1. Open the n11.js file and configure any settings, such as:
  - Path to Chrome/Chromium
  - Output CSV location
  - User agents for web scraping

2.Run the scraper:
```bash
node n11.js
```
3.The scraped data will be saved as a CSV file in the specified directory (default: ../../Data_Analysis/csv/).

🗂️ Output
The CSV file includes the following columns:
  - productId: Unique identifier for each product.
  - productTitle: Name of the product.
  - price: Price of the product.
  - productUrl: URL of the product page.
  - imageSrcset: URL of the product image.
  - ProductCategory: Main category of the product.
  - SubCategory: Subcategory of the product.

📚 Dependencies
Puppeteer: Headless browser automation library.
fast-csv: A library for parsing and writing CSV files.

📝 Notes
Ensure that you have a stable internet connection while running the scraper.
The scraper runs in non-headless mode by default to facilitate debugging. To enable headless mode, adjust the Puppeteer launch settings in n11.js.
Adjust random delay timings in the script to mimic human-like interactions.

> [!WARNING]  
> Puppeteer requires the path to your Chrome executable. For Windows, update the executablePath in the script to the default Chrome location:
> ```bash
>executablePath: 'C:\\Program Files\\Google\\Chrome\\Application\\chrome.exe'
> ```

🎉 Happy scraping! 🚀
