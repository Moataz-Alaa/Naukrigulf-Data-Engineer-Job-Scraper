# Naukrigulf Data Engineer Job Scraper

## 📖 Overview
This project is a Python-based web scraping tool built using **Selenium**. It automates the process of navigating the **Naukrigulf** job portal to extract detailed information for "Data Engineer" job listings. The script dynamically handles pagination, scraping data from the first three pages of search results, and exports the collected data into a structured CSV file.

## ✨ Features
- **Automated Navigation**: Uses Selenium WebDriver to interact with the live Naukrigulf website.
- **Dynamic Pagination**: Automatically navigates through the first 3 pages of the search results.
- **Detailed Extraction**: Clicks into individual job postings to scrape the full job description.
- **Data Structuring**: Cleans and organizes the scraped data into a well-structured CSV format.

## 📊 Extracted Data
For every job listing found on pages 1, 2, and 3, the script extracts the following fields:
1. **Job Title**
2. **Company Name**
3. **Job Location**
4. **Required Experience**
5. **Full Job Description**

## 🛠️ Prerequisites
Before running the script, ensure you have the following installed:
- Python 3.7 or higher
- Google Chrome Browser
- Jupyter Notebook or JupyterLab

## 📦 Installation

1. **Clone the repository** (or download the project files):
   ```bash
   git clone <repository-url>
   cd <project-folder>
   ```

2. **Install required Python packages**:
   Create a virtual environment (optional but recommended) and install the dependencies:
   ```bash
    pip install selenium webdriver-manager pandas jupyter
   ```
   *(Note: webdriver-manager is used to automatically handle the browser driver binaries, pandas is used for easy CSV export, and jupyter is required to run the notebook).*

## 🚀 Usage

1. Launch Jupyter Notebook from your terminal in the project directory:
   ```bash
   jupyter notebook
   ```
   *(Or use `jupyter lab` if you prefer JupyterLab).*

2. Your default web browser will open with the Jupyter file tree. Navigate to and open the **`Naukrigulf_DataEngineer_Scraper.ipynb`** file.

3. Run the cells sequentially by clicking the "Run" button or pressing `Shift + Enter`. 
   - *Tip: You can also go to the top menu and select **Cell -> Run All** to execute the entire scraping process at once.*

4. The script will launch a browser, navigate to Naukrigulf, search for "Data Engineer", and begin scraping. Once completed, the browser will close automatically.

## 📂 Output
Upon successful execution, the script will generate a CSV file named **`data_engineer_jobs.csv`** in the project directory. 

The CSV will contain the following columns:
| Job Title | Company Name | Job Location | Required Experience | Job Description |
| :--- | :--- | :--- | :--- | :--- |
| Data Engineer | XYZ Corp | Dubai, UAE | 3-5 Years | [The job description...] |

## ⚠️ Disclaimer
This script is intended for **educational purposes only**. 
- Web scraping may violate the Terms of Service of certain websites. 
- Please use this tool responsibly and ensure you comply with Naukrigulf's `robots.txt` and terms of use.
- Avoid sending too many rapid requests to prevent overloading their servers or getting your IP blocked.
