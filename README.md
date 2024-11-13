# Web Scraping and Data Analysis in Python

## Project Description
This project demonstrates the use of Python for web scraping and data analysis. By extracting a table from Wikipedia, the project processes company revenue data and performs data cleaning and analysis. This enables insights into the largest companies in the U.S., including ranking, industry distribution, and revenue trends.

## Features
- Fetches and parses HTML content from Wikipedia.
- Extracts a table containing information about the largest companies in the U.S. by revenue.
- Cleans and processes the scraped data.
- Performs data analysis to summarize insights.
- Visualizes data for better interpretation.

## Data Analysis
The analysis focuses on:
1. **Industry Breakdown**: 
   - Categorizes companies by industry and shows the distribution.
2. **Revenue Trends**:
   - Identifies the company with the highest and lowest revenue.
   - Calculates the average and total revenue for the dataset.
3. **Employee Data**:
   - Summarizes the total number of employees across all companies.
4. **Geographical Insights**:
   - Analyzes the distribution of company headquarters.

### Key Findings
- The **largest company by revenue** is **Walmart**, with a revenue of **$572,754 million**.
- The **industry with the most representation** is **Retail**, appearing 1 time in this dataset.
- The **average revenue** across the dataset is approximately **$469,464 million**.
- The **total number of employees** across all companies is **4,062,000**.
- The most common **headquarters location** is **Bentonville, Arkansas**.

### Visualizations
The notebook includes:
- **Bar Charts** for company revenue ranking.
- **Pie Chart** showing industry distribution.
- **Histogram** to visualize employee count distribution.

Example chart:
```python
import matplotlib.pyplot as plt

# Example: Industry distribution pie chart
industry_counts = df['Industry'].value_counts()
industry_counts.plot(kind='pie', autopct='%1.1f%%', figsize=(8, 8))
plt.title('Industry Distribution')
plt.show()
```

## Requirements
- Python 3.7 or above
- Libraries:
  - `requests`
  - `beautifulsoup4`
  - `pandas`
  - `matplotlib`

## Installation
1. Clone this repository:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Open the Jupyter Notebook file:
   ```bash
   jupyter notebook [PROJECT]_Web_Scraping_in_Python.ipynb
   ```

2. Run the notebook to:
   - Scrape the Wikipedia page.
   - Clean and process the data.
   - Perform analysis and generate visualizations.

## File Structure
- `notebook.ipynb`: Main Jupyter Notebook with web scraping and data analysis code.
- `requirements.txt`: List of Python dependencies.
- `README.md`: Documentation for the project.
