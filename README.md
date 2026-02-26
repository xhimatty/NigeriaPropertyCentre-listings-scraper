# Resilient Multi-Page Property Listings Scraper for NigeriaPropertyCentre

A web scraping tool to systematically collect property data (title, address, price, agent, bedroom/bathroom/toilet/parking/SQM, and listing URL) across multiple pages and cities. Supports flexible search filters, error-resilient extraction, structured retry handling, and automated post-scrape data normalization using Pandas.

![image](https://github.com/user-attachments/assets/7a55c2a0-4ceb-45ed-a5e6-f99651dae5da)

### Project Summary
Developed a robust Python-based web scraping pipeline using Playwright to extract multi-page property listings from NigeriaPropertyCentre.com. The scraper handles dynamic content, DOM manipulation, intermittent page failures with safe retry logic, and structured URL enrichment. A post-processing data cleaning layer standardizes currency values and textual metadata, producing both raw and normalized CSV datasets suitable for analytics or integration into broader data processing systems.

### Key Features
- Multi-page property listings extraction
- Dynamic user-agent rotation to reduce detection
- DOM element inspection for precise attribute-level data extraction
- Safe retry logic with incremental backoff for page load failures
- Efficient error handling to maintain scraper continuity
- Flexible search filters: listing type, city, bedroom count
- Canonical URL construction and enrichment for each listing
- Regex-based currency sanitization and numeric price normalization
- Text normalization (whitespace cleanup, non-breaking space handling)
- Dual dataset output:
    Raw scraped CSV
    Cleaned and normalized CSV
- Randomized delays to mimic human interaction and reduce detection risk

### Tech Stack
    Language: Python 3.x
    Automation & Scraping: Playwright
    Data Processing & Cleaning: Pandas, Regex
    Resilience Handling: Incremental retry/backoff logic
    Output: Structured CSV (raw and cleaned datasets)

