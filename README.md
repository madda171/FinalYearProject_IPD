# FinalYearProject_IPD
Interim Progress Report Codes + ReadMe File

Certainly! Below is a sample README file that explains the purpose of the code, how to set it up, and how to use it.

---

# Sector Data Merging Script

## Overview

This Python script is designed to extract sector data from a ZIP file containing multiple CSV files and merge it with a main dataset containing market capitalization information. The resulting merged dataset will include sector information for each symbol in the main dataset.

## Requirements

- Python 3.x
- Pandas library
- Zipfile library (included in Python standard library)
- OS library (included in Python standard library)

## Installation

1. Ensure you have Python installed on your machine. You can download it from [python.org](https://www.python.org/downloads/).
2. Install the Pandas library if you haven't already. You can do this using pip:

   ```bash
   pip install pandas
   ```

## Usage

1. **Prepare Your Files:**
   - Place your ZIP file containing the sector data in the appropriate directory. Update the `zip_path` variable in the script to point to your ZIP file.
   - Ensure you have your main dataset (e.g., `market-capitalization.csv`) in the specified path. Update the `main_df_path` variable in the script to point to your main dataset.

2. **Run the Script:**
   - Execute the script in your Python environment. You can run it in a Jupyter notebook, a Python script file, or any other Python IDE.

   ```bash
   python your_script_name.py
   ```

3. **Output:**
   - The script will extract all CSV files from the ZIP file, merge the sector information into the main dataset based on the 'Symbol' column, and save the final merged dataset as `merged_data.csv` in the current directory.

## Code Explanation

- The script begins by importing necessary libraries (`pandas`, `zipfile`, and `os`).
- It defines file paths for the ZIP file and the main dataset.
- The ZIP file is extracted into a folder named `extracted_data`.
