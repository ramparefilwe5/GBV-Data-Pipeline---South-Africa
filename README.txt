GBV DATA PIPELINE - SOUTH AFRICA
=================================

A data engineering project that collects, processes, and visualizes
Gender-Based Violence (GBV) statistics across South Africa.

DESCRIPTION
-----------
This project scrapes GBV data from public sources (SAPS reports, StatsSA,
news articles), cleans and stores it in a database, and provides a web
dashboard with interactive charts and downloadable reports.

The goal is to create a centralized resource for understanding GBV trends
in South Africa to support research and awareness.

DATA SOURCES
------------
- SAPS (South African Police Service) annual crime statistics
- StatsSA (Statistics South Africa) population data
- News articles from News24, IOL, SABC News

FEATURES
--------
- Web scraping for automated data collection
- Data cleaning and transformation pipeline
- PostgreSQL/SQLite database storage
- Interactive web dashboard with charts
- Provincial comparison maps
- PDF report generation
- REST API for data access

TECH STACK
----------
- Language:    Python 3.12
- Scraping:    BeautifulSoup4, Requests
- Processing:  Pandas, NumPy
- Database:    SQLite / PostgreSQL
- Web:         Flask, Chart.js
- Reports:     ReportLab

SETUP INSTRUCTIONS
------------------
1. Clone the repository
2. Install dependencies: pip install -r requirements.txt
3. Initialize database: python database/init_db.py
4. Run scraper: python scraper/saps_scraper.py
5. Start web app: python web/app.py
6. Open browser: http://localhost:5000

PROJECT STRUCTURE
-----------------
gbv-data-pipeline/
├── scraper/          # Web scraping scripts
├── data/raw/         # Raw scraped data
├── pipeline/         # Data cleaning and loading
├── database/         # Database setup and queries
├── web/              # Flask web application
├── reports/          # PDF report generation
└── requirements.txt  # Python dependencies

AUTHOR
------
Refilwe Rampare
Data Engineering Elective Project
