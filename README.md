# Flipkart Review Scraper

A web application to scrape and display product reviews from Flipkart using Python, Flask, and BeautifulSoup.

## Features

- Enter a product name and fetch the latest reviews directly from Flipkart.
- Displays reviews with product name, customer name, rating, comment heading, and the comment itself.
- Responsive and clean UI using HTML and CSS.
- Stores reviews (optional, MongoDB integration present but commented out).

## How It Works

1. Enter a product name in the search form.
2. The app scrapes Flipkart search results for the product and fetches its review page.
3. Extracts relevant review details and displays them in a table.


## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/GirishSonune/GirishSonune-Flipkart_Review_scrap.git
cd GirishSonune-Flipkart_Review_scrap
```

### 2. Create and activate a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate   # for Linux/macOS
venv\Scripts\activate      # for Windows
```

### 3. Install requirements

```bash
pip install -r requirements.txt
```

### 4. Run the application

```bash
python app.py
```

Then, visit [http://localhost:5000](http://localhost:5000) in your browser.

## Configuration

- **MongoDB Integration:**  
  The code includes optional MongoDB integration (currently commented out).  
  To enable:
  - Set up a MongoDB database (local or Atlas).
  - Update the MongoDB URI in `app.py`.
  - Uncomment the relevant lines to store reviews in the database.

## Project Structure

```
.
├── app.py
├── requirements.txt
├── templates/
│   ├── base.html
│   ├── index.html
│   └── result.html
├── static/
│   └── css/
│       ├── main.css
│       └── style.css
└── scrapper.log
```

## Dependencies

- Flask
- Flask-CORS
- requests
- beautifulsoup4
- pymongo (optional, for MongoDB integration)

Install all dependencies using:

```bash
pip install -r requirements.txt
```

## Notes

- This app is for educational/demo purposes only.  
- Flipkart's website structure may change, which could break the scraper.  
- Respect Flipkart's terms of service and robots.txt.

## License

MIT License

---

*Made with ❤️ by [Girish Sonune](https://github.com/GirishSonune)*
