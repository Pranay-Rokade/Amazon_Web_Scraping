# Amazon_Web_Scraping 🛒

## 📌 Overview

This project is a **Python-based Amazon Web Scraper** that extracts product details from Amazon search results using **BeautifulSoup** and **Requests**. The extracted data includes:

- **Product Name**
- **Price**
- **Rating**
- **Seller Name** (Fetched from the product detail page)

The extracted data is then stored in a **CSV file** for further analysis.

---

## 🚀 Features

- Extracts multiple product details from Amazon's search results.
- Fetches the **seller name** by visiting each product's detail page.
- Saves the scraped data in a structured **CSV file**.
- Uses headers to mimic a real browser request and avoid detection.

---

## 📂 Project Structure

```
Amazon-Scraper/
│── amazon_scraper.py   # Main script for scraping Amazon
│── amazon_products.csv # Output file storing scraped data
│── README.md           # Project documentation
```

---

## 🔧 Prerequisites

Ensure you have **Python 3.x** installed on your system.

Install the required dependencies using:

```bash
pip install requests beautifulsoup4
```

---

## 🛠️ How It Works

### 1️⃣ Fetch Amazon Search Results

The script sends a request to Amazon's search page and extracts product details such as:

- Product Name
- Price
- Rating
- Seller Name

### 2️⃣ Fetch Seller Name from Product Page

Since Amazon does not display seller names on the search page, the script visits each product’s detail page and extracts the seller’s name from the **'Sold by'** section.

### 3️⃣ Save Data to CSV

All extracted product information is stored in `amazon_products.csv` for further analysis.

---
