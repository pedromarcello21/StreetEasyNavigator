# StreetEasy Navigator

## Overview

The **StreetEasy Navigator** is a CLI app that allows users to scrape apartment listings from StreetEasy based on their budget, preferred number of bedrooms, and selected neighborhoods. The listings are exported to an Excel file with clickable links for easy access to the apartment details.

## Features

- **User Input:** Users can input their budget, number of bedrooms, and desired neighborhoods to filter the listings.
- **Web Scraping:** The tool uses Selenium and BeautifulSoup to navigate the StreetEasy website, scrape relevant apartment data, and avoid bot detection.
- **Data Export:** The scraped data is exported to an Excel file with hyperlinks to the apartment listings for easy access.
- **Error Handling:** Built-in error handling to ensure smooth execution, even with invalid inputs or unexpected website changes.

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/streeteasy-navigator.git
   cd streeteasy-navigator
   ```

2. **Install Dependencies:**
   Make sure you have Python installed. Install the required Python libraries using pip:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up ChromeDriver:**
   Ensure you have ChromeDriver installed and it's accessible in your system's PATH. You can download it from [here](https://sites.google.com/a/chromium.org/chromedriver/downloads).

## Usage

1. **Run the Application:**
   Start the scraper by running the Python script:
   ```bash
   python streeteasy_navigator.py
   ```

2. **Provide Inputs:**
   - **Budget:** Enter your maximum budget (e.g., `2000` for $2000). Minimum budget is $500.
   - **Bedrooms:** Enter the number of bedrooms (e.g., `1`, `2`, `Studio`).
   - **Neighborhoods:** Enter the neighborhoods you're interested in, separated by commas (e.g., `Upper East Side, Williamsburg`).

3. **Results:**
   The script will scrape the listings and generate an Excel file with the current date in the filename (e.g., `August 10 2024 Listings.xlsx`). The file will contain the apartment addresses, prices, fees, and clickable links to the listings.

## Example Output

An example output Excel file might look like:

| Address                             | Price    | Fee    | Link                                             |
|-------------------------------------|----------|--------|--------------------------------------------------|
| 123 Main St, Upper East Side        | $2,000   | No Fee | [Link](https://streeteasy.com/listing/123-main)  |
| 456 Park Ave, Williamsburg           | $1,800   | FEE    | [Link](https://streeteasy.com/listing/456-park)  |

## Known Issues

- **Bot Detection:** The script includes measures to avoid bot detection, but in some cases, it may still be blocked. If this happens, try running the script again or implementing additional anti-bot strategies.



This project is licensed under the MIT License.
```

You can copy and paste this directly into your GitHub repository's README.md file! Let me know if you need any more adjustments.
