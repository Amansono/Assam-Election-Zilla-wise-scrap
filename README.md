# Assam Panchayat Electoral Roll - Full State Scraper
This repository contains a specialized Selenium-based scraper designed to map the entire electoral hierarchy of Assam's Panchayat system. It traverses every District, Zila Parishad, Gaon Panchayat, and Ward to compile a master list of Polling Stations.

## Scope: All in Assam
This script is configured to scrape all **27+ Districts** under the Assam Panchayat Act, covering:
* **~400** Zila Parishad Constituencies (ZPC)
* **~2,200** Gaon Panchayats (GP)
* **~22,000** Wards
* **~25,000+** Polling Stations (Booths)

## Technical Workflow
The scraper uses a deep-nested loop logic with **Force-Selection** to handle the state-dependent dropdowns on the ERMS Assam portal:
1. **District Level:** Initializes the session.
2. **ZPC Level:** Refreshes based on District choice.
3. **GP Level:** Filters based on ZPC.
4. **Ward Level:** Pulls specific ward boundaries.
5. **Booth Level:** Extracts the final Polling Station data.

## Setup & Requirements
```bash
pip install selenium beautifulsoup4 pandas openpyxl
