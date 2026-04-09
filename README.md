This Python script automates the extraction of electoral roll metadata from the ERMS Assam portal. It navigates through nested dropdown selections to compile a complete mapping of Districts, Zila Parishads, Gaon Panchayats, Wards, and Polling Stations into an Excel file.

📋 Features
Hierarchical Scraping: Automatically handles dependent dropdowns.

Resilient Selection: Uses a force_select mechanism to ensure the UI updates before proceeding.

Data Export: Saves progress to a .xlsx file using pandas.

Clean Exit: Ensures the browser closes and data is saved even if an error occurs.

🛠️ Prerequisites
Before running the script, ensure you have the following installed:

Python 3.8+

Selenium: For browser automation.

BeautifulSoup4: For fast parsing of dropdown options.

Pandas & Openpyxl: For data manipulation and Excel export.

Webdriver: (e.g., ChromeDriver) matching your browser version.
