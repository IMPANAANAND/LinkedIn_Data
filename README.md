# LinkedIn Company Authenticity & Data Scraper

This Jupyter Notebook automates the process of scraping and analyzing LinkedIn company pages to assess their authenticity and extract key company information, including leaders and affiliated pages.

## Features

- **Authenticity Analysis:**  
  Scrapes company data from LinkedIn and the company's website to evaluate authenticity using multiple indicators (domain info, SSL, website professionalism, jobs, posts, etc.).

- **Section Scraping:**  
  Extracts company leaders and affiliated pages from the LinkedIn "Life" section.

- **Sentiment Analysis:**  
  Uses a BERT-based model to analyze the sentiment and professionalism of company posts.

- **Comprehensive Output:**  
  Saves all results in a structured JSON file for further use.

## Requirements

- Python 3.7+
- Google Chrome browser
- ChromeDriver (automatically managed by `webdriver_manager`)
- The following Python packages:
  - selenium
  - webdriver_manager
  - beautifulsoup4
  - requests
  - whois
  - transformers
  - torch
  - pandas
  - scikit-learn
  - logging

Install dependencies with:

```sh
pip install selenium webdriver_manager beautifulsoup4 requests python-whois transformers torch pandas scikit-learn
```

## Usage

1. **Run the Notebook:**  
   Open `Linkedin Scrape Final 1.ipynb` in Jupyter or VS Code.

2. **Input LinkedIn URL:**  
   When prompted, enter the LinkedIn company URL (e.g., `https://www.linkedin.com/company/yahoo/`).

3. **Wait for Analysis:**  
   The notebook will scrape data, analyze authenticity, and extract leaders and affiliated pages.

4. **Output:**  
   Results are saved as a JSON file named `<company_name>_company_data.json` in the current directory.

## Notes

- **LinkedIn Restrictions:**  
  Some data may be limited due to LinkedIn's anti-bot measures or login requirements.
- **Ethical Use:**  
  Use this tool responsibly and in compliance with LinkedIn's terms of service.

## File Structure

 Main notebook containing all scraping and analysis logic.

## Logging

Logs are printed to the console for debugging and error tracing.

## License

This project is for educational and research purposes only.
