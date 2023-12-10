# Data-Acquisition-and-Preprocessing

# Project Documentation: Web Scraping of Highly-Ranked Films

# Overview
The project comprises a Python-based automated script that collects data on top-rated films from one website. The data is retrieved, formatted, and it is saved to a csv file and an accompanying SQLite database.

# Purpose

This script is intended to gather data of high rated films for either in analyses or for display purposes.

# Technologies

- Python 
- Libraries: BeautifulSoup (bs4), Pandas, SQLite3 library.

# Installation and Setup
# Prerequisites

- The system had python 3.x.
- Required Python packages: requests, beautifulsoup4, pandas

To install these packages, run:

pip install requests beautifulsoup4 pandas

# Running the Script

1. Duplicate and copy the script on your computer locally.
2. Open a terminal or command prompt and navigate to the directory containing your script.
3. Run the script using Python:

python webscraping_py.py



# Script Details
Web Scraping

- URL: Specifically, the script aims at attacking certain URL with an index of 100 best movies.
- Data Extraction: Parses HTML, requesting movie information using BeautifulSoup.

Data Processing

- Data Structure: Each row of data is organized into a DataFrame consisting three columns labeled Average Rank, Film and Year.
- Limitation: It only processes a maximum of fifty films among the best.

Output

- CSV Output: Data is stored in a .csv file named top_50_films.csv.
- SQLite Database: Data is also saved into a SQLite database called “movies.db” and a table named “Top_50”.
Code Explanation
Import Statements

- The script enables access to relevant libraries for the purposes of performing HTTP requests, parsing HTML, processing data, and handling database operations.

Main Logic

- For a script, the process starts with fetching the HTML contents of the page from which it pars through fifty initial rows from the main table and acquires film data.
- Finally, extracted information is appended to a pandas DataFrame.

Data Storage

- Print the DataFrame to the console to confirm.
- The results are also written in a CSV file as well as to a SQLite database.




Limitations and Future Improvements
Limitations: In the present, it scripts are confined for a specific linkage structure and table format.
Future Improvements:

- Modify the script to accommodate various table forms or several URLs.
- Handle errors associated with the net or HTML structure.
- Develop new methods to update old database entries instead of replace them.
