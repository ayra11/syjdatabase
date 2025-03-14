# 51job Data Analysis

## Introduction
This project analyzes job postings from the Chinese recruitment website **51job**. Data was collected using web scraping, and only a small sample was used for analysis. The dataset consists of two main parts: **primary data** and **detailed data**.

## Data Source
The data comes from **51job**, one of the largest job recruitment websites in China. Web scraping techniques were employed to extract job postings, ensuring that only a subset of the total data was used.

## Dataset Structure

### Primary Data
The **primary data** includes the following fields:
- **Title** (职位标题)
- **Title Link** (职位链接)
- **Region** (地区)
- **Province/City** (省/城市)
- **Prefecture-Level City** (地级城市)
- **Work Experience** (工作经验)
- **Work Experience (Float)** (工作经验_float)
- **Education Level** (学历)
- **Education Level (Int)** (学历_int)
- **Company Name** (公司名称)
- **Company Type** (公司性质)
- **Company Size** (公司规模)
- **Industry (First-Level Segment)** (行业领域_第一段)
- **National Economic Industry Classification** (国民经济行业分类)
- **Salary** (薪资)
- **Lower Salary Range** (薪资下区间)
- **Upper Salary Range** (薪资上区间)
- **Salary Unit** (薪资单位)
- **Job Function (Subcategory)** (职能中类)
- **Job Function (Major Category)** (职能大类)
- **Posting Date** (发布时间)
- **Year** (年份)
- **Data Collection Timestamp** (采集时的时间)

### Detailed Data
The **detailed data** includes:
- **Job Description** (职位信息)
- **Word Segmentation** (分词)

## Analysis Components

### Data Analysis
1. **Data Loading and Structure Overview**
   - The dataset is loaded from a CSV file (`jobposting sample.csv`).
   - Columns are predefined and checked for completeness.
   - A summary table is created to show missing values in each column.

2. **Data Cleaning**
   - The `发布时间` (posting date) column is cleaned by removing unnecessary characters.
   - The `年份` (year) and `发布时间` (posting date) columns are merged to create a new complete date column.

3. **Data Summary**
   - Basic statistics such as row counts and missing data are analyzed.
   - The dataset’s overall consistency is checked.

### Job Analysis
1. **Industry and Job Function Analysis**
   - Job postings are categorized by industry (`行业领域_第一段` and `国民经济行业分类`).
   - Job functions (`职能中类` and `职能大类`) are analyzed to determine demand trends.

2. **Salary Analysis**
   - The salary range (`薪资下区间`, `薪资上区间`) is examined to understand wage distribution.
   - Different salary trends across industries and job functions are analyzed.

3. **Geographical Trends**
   - Job postings are grouped by region (`省/城市`, `地级城市`) to analyze location-based employment trends.
   - Heatmaps or charts may be generated to visualize job distribution.

## Usage
To use this project, ensure you have the necessary Python libraries installed. Open the provided Jupyter Notebook and follow the analysis steps.

## Dependencies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- BeautifulSoup (for web scraping)
- Requests

## Acknowledgments
This project is based on publicly available job postings from **51job**. The data was collected solely for academic and analytical purposes.

