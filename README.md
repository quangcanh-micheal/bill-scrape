# bill-scrape
This project is an automated data collection and image retrieval pipeline developed for an Upwork client to gather localized visual evidence of financial transactions (receipts and bills) across various countries. The system automates the process of translating search terms, generating localized queries, and harvesting image URLs from travel and review platforms.

# Project Files Overview
bill_scrape.ipynb (The Automation Engine): This notebook contains the core logic for the project. It uses pandas to manage a database of countries and languages, and integrates with the SerpApi Google Search API to programmatically perform image searches. The script iterates through a list of locations, executes specific queries (targeting platforms like TripAdvisor and Reddit), and extracts the top five direct image links for each entry.

bill_scrape.xlsx - Sheet1.csv (The Global Dataset): This file serves as both the input configuration and the final output for the project. It contains:

Geographic Metadata: Country, language, and capital city.

Translation Logic: Localized terms for "Receipt" (e.g., Kvittering for Denmark, Rechnungen for Germany).

Search Strings: Pre-formatted queries designed to find receipts in specific cities on travel forums.

Harvested Results: Columns (img_1 through img_5) containing the direct URLs of the images retrieved by the script.
