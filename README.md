# COVID-19 Global Data Tracker

## Project Overview

This project is a data analysis report that tracks the global trends of COVID-19 using real-world data. It focuses on exploring time-based and geographical patterns in infections, deaths, and vaccinations across selected countries. The goal is to gain insights and understand how the pandemic has evolved over time in different regions.

This analysis uses the official dataset from "Our World in Data", and is implemented using Python in a Jupyter Notebook environment (Google Colab). The project follows a step-by-step approach including data collection, cleaning, exploratory data analysis, visualization, and reporting of key findings.

---

## Objectives

- Import and clean real-world COVID-19 data.
- Analyze trends in daily new cases and deaths.
- Compare the progression of the pandemic across countries.
- Visualize key metrics using charts and graphs.
- Evaluate vaccination progress in selected countries.
- Draw insights and highlight notable patterns from the data.

---

## Dataset

**Source:**  
Our World in Data - COVID-19 Dataset  
URL: [https://ourworldindata.org/covid-deaths](https://ourworldindata.org/covid-deaths)

**File Used:**  
`owid-covid-data.csv`

**Key Columns Used:**

- `date`
- `location`
- `new_cases`
- `new_deaths`
- `total_cases`
- `total_deaths`
- `total_vaccinations`

---

## Technologies and Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab (Jupyter Notebook)

---

## Project Workflow

### 1. Data Collection

- The dataset was downloaded from the Our World in Data COVID-19 repository as a CSV file.
- It contains COVID-19 related statistics from multiple countries over time.

### 2. Data Loading and Initial Exploration

- The dataset is loaded using `pandas.read_csv()`.
- An overview of columns and missing values is generated.
- Basic exploration is done using `.head()`, `.info()`, and `.isnull().sum()`.

### 3. Data Cleaning

- Filtered the dataset to focus on three countries: Kenya, United States, and India.
- Converted the `date` column to proper datetime format using `pd.to_datetime()`.
- Dropped rows with missing values in critical columns (`new_cases`, `new_deaths`).
- Missing values in `total_vaccinations` were filled with zeros for clarity in charts.

### 4. Exploratory Data Analysis (EDA)

- **Line charts** to track daily new cases and total deaths over time.
- **Bar chart** to show average daily new cases by country.
- **Scatter plot** to explore the relationship between new cases and new deaths.

### 5. Vaccination Analysis

- A separate line plot to show vaccination progress for each selected country.
- Helped to understand the pace and timing of vaccine rollout.

### 6. Insights and Observations

Key insights from the data include:

- The United States consistently recorded higher daily new cases than Kenya and India.
- Kenya had significantly fewer cases and deaths compared to the other countries.
- Vaccination rollouts started at different times, with the United States ahead of the others.
- The relationship between new cases and new deaths suggests that spikes in cases are often followed by increases in deaths.

---

## How to Use This Notebook

1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Upload the `owid-covid-data.csv` using the upload button or the file upload code.
3. Run the cells one by one.
4. Examine the visualizations and read the markdown commentary to understand the findings.

---

## Directory Structure

- **covid19_global_tracker.ipynb**: Main Jupyter Notebook file.
- **owid-covid-data.csv**: Raw COVID-19 dataset (not included in repo).
- **README.md**: Project documentation.



## License

This project is open-source and available under the MIT License.

---

## Acknowledgments

- Our World in Data for providing the comprehensive and up-to-date COVID-19 dataset.
- The open-source Python and data science communities for their tools and libraries.

## Author
Joy Wanjiru Simiyu.






