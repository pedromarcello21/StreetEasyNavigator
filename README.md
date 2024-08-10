StreetEasy Scraper CLI
Overview
The StreetEasy Scraper CLI is a Python-based command-line application that allows users to scrape apartment listings from StreetEasy based on their budget, preferred number of bedrooms, and selected neighborhoods. The listings are exported to an Excel file with clickable links for easy access to the apartment details.

Features
User Input: Users can input their budget, number of bedrooms, and desired neighborhoods to filter the listings.
Web Scraping: The tool uses Selenium and BeautifulSoup to navigate the StreetEasy website, scrape relevant apartment data, and avoid bot detection.
Data Export: The scraped data is exported to an Excel file with hyperlinks to the apartment listings for easy access.
Error Handling: Built-in error handling to ensure smooth execution, even with invalid inputs or unexpected website changes.
Installation
Clone the Repository:

bash
Copy code
git clone https://github.com/your-username/streeteasy-scraper-cli.git
cd streeteasy-scraper-cli
Install Dependencies:
Make sure you have Python installed. Install the required Python libraries using pip:

bash
Copy code
pip install -r requirements.txt
Set Up ChromeDriver:
Ensure you have ChromeDriver installed and it's accessible in your system's PATH. You can download it from here.

Usage
Run the Application:
Start the scraper by running the Python script:

bash
Copy code
python streeteasy_scraper.py
Provide Inputs:

Budget: Enter your maximum budget (e.g., 2000 for $2000). Minimum budget is $500.
Bedrooms: Enter the number of bedrooms (e.g., 1, 2, Studio).
Neighborhoods: Enter the neighborhoods you're interested in, separated by commas (e.g., Upper East Side, Williamsburg).
Results:
The script will scrape the listings and generate an Excel file with the current date in the filename (e.g., August 10 2024 Listings.xlsx). The file will contain the apartment addresses, prices, fees, and clickable links to the listings.

Example Output
An example output Excel file might look like:

Address	Price	Fee	Link
123 Main St, Upper East Side	$2,000	No Fee	Link
456 Park Ave, Williamsburg	$1,800	FEE	Link
Known Issues
Bot Detection: The script includes measures to avoid bot detection, but in some cases, it may still be blocked. If this happens, try running the script again or implementing additional anti-bot strategies.
