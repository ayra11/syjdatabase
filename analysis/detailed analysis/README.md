# Job Split Analysis

## Table of Contents
- [Overview](#Overview)
- [Data Source](#data-source)
- [Analysis Components](#analysis-components)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Related Work](#acknowledgments)

## Overview
This project focuses on extracting major-related information from job postings to accurately determine the corresponding undergraduate major for each position. The dataset used in this analysis is the same as in the **Basic Analysis** folder. Please refer to that folder for detailed information about data collection and preprocessing.

## Data Source
The data used in this project is scraped from the **51job** website, containing job postings and relevant details.

## Analysis Contents
### Data Preprocessing
- **Text Cleaning with Regular Expressions (Regex)**: Removing noise and unnecessary characters from job postings.
- **Keyword-Based Information Extraction**: Identifying key major-related terms using a non-overlapping keyword matching technique.
- **Data Deduplication & Formatting**: Handling duplicates, missing values, and standardizing text formats.

### Job Classification
- **Major Extraction**: Extracting major-related information from job descriptions to determine the most relevant undergraduate discipline.
- **Rule-Based Classification**: Assigning job categories based on predefined keyword lists.
- **Frequency Analysis**: Utilizing `collections.Counter` to determine common job-related terms.
- **Text Processing for NLP**: Implementing stopword removal and tokenization to improve classification accuracy.

## Usage
Run the Jupyter Notebook (`job split.ipynb`) to reproduce the analysis.

## Dependencies
Ensure the following Python libraries are installed:
```bash
pip install pandas numpy matplotlib seaborn
```

## Related Work
For foundational analysis, refer to the **Basic Analysis** folder, which provides detailed information about the dataset and initial exploratory analysis.

