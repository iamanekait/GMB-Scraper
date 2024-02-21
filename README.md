# Google Maps Business Scraper

This Python script allows you to scrape business information from Google Maps using Playwright. It retrieves business names, addresses, websites, phone numbers, and reviews (if needed) based on the search keywords provided.

## Requirements
- Python 3.6+
- Playwright library (`pip install playwright`)
- Pandas library (`pip install pandas`)

## Installation
1. Clone this repository or download the script.
2. Install the required libraries using pip:
    ```
    pip install playwright pandas
    ```

## Usage
1. Run the script from your terminal or command prompt:
    ```
    python google_maps_scraper.py
    ```
2. Enter the search keywords when prompted.
3. Input the total number of business listings to scrape.
4. The script will launch a browser window (non-headless for debugging purposes), perform the search, scrape the business information, and save it to both Excel (.xlsx) and CSV (.csv) files.

## Script Details
- The script utilizes Playwright to interact with the Google Maps web interface.
- It scrapes business information such as name, address, website, and phone number.
- Optionally, it can also scrape reviews, although this feature is currently commented out.
- The scraped data is stored in `Business` data class objects and then converted to pandas DataFrame for easy manipulation and saving to files.

Feel free to customize the script according to your specific needs and requirements!

**Note:** Make sure to adjust the CSV file path (`business_list.save_to_csv("Put your path.csv")`) according to your system configuration.
