# 🎬 Netflix Dataset Analysis with Python

Exploratory data analysis of Netflix Movies and TV Shows, built with Python and pandas as part of a Data Analytics course project.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/abdumannopovadurdona56-afk/data-analysis-project/blob/main/netflixAnalyticsProject_(1).ipynb)

**Author:** Abdumannopova Durdona
**Course:** Data Analytics (24-301)
**Instructor:** Nilufar Nosirjonova

---

## 📌 Project Description

This project analyzes a real-world dataset of Netflix Movies and TV Shows collected from Flixable. The dataset includes metadata such as title, category, director, cast, country, release year, rating, duration, and genre.

The goal was to explore content distribution patterns, identify trends over time, examine content ratings, and extract meaningful insights about Netflix's catalog using Python and pandas.

The analysis covers **data cleaning, exploratory data analysis (EDA), filtering, grouping, sorting, and visualization**.

## 🎯 Objectives

- Practice real-world data analysis using Python and pandas
- Apply filtering, grouping, and sorting techniques
- Perform exploratory data analysis (EDA)
- Create visualizations using matplotlib / seaborn
- Extract meaningful insights from the dataset
- Present results clearly using code, comments, and graphs

## 🗂️ Dataset

The dataset contains information about movies and TV shows available on Netflix.

| Column | Description |
|---|---|
| Show_Id | Unique identifier |
| Title | Name of the movie/show |
| Category | Movie or TV Show |
| Director | Director name |
| Cast | Cast members |
| Country | Country of production |
| Release_Date / Year | Release date |
| Rating | Content rating (e.g. TV-14, R) |
| Duration | Length (minutes or seasons) |
| Type | Genre |

## 🛠️ Tools & Technologies

- Python
- Pandas
- Matplotlib / Seaborn
- Jupyter Notebook / Google Colab

## 🧹 Data Cleaning

Before analysis, the dataset was cleaned to ensure accuracy and consistency:

1. Checked for missing values
2. Replaced missing values in `Director`, `Cast`, `Country`, `Rating`, `Type`, `Description` with `"Unknown"`
3. Converted `Release_Date` to a proper datetime format
4. Dropped rows with missing critical fields (`Title`, `Category`, `Release_Date`, `Duration`)
5. Removed duplicate records
6. Extracted numeric values from the `Duration` column for numerical analysis

## 🔍 Analysis Tasks

The notebook works through 13 guided analysis tasks, including:

1. Look up a specific title's Show ID and Director
2. Find the year with the highest number of releases (bar chart)
3. Count Movies vs. TV Shows (bar chart)
4. Filter Movies released in a specific year
5. List TV Shows released in India
6. Find the Top 10 Directors by number of titles (bar chart)
7. Filter by Category, Type, and Country combinations
8. Search for titles featuring a specific cast member
9. Identify all rating categories, and filter by rating + country + year
10. Determine the maximum duration of a Movie and a TV Show
11. Sort the dataset by release year
12. Combine multiple category/type conditions with OR logic

Each task includes the pandas code used, along with a short written interpretation of the result.

## 📊 Exploratory Data Analysis

- **Movies vs. TV Shows distribution** — Movies make up the majority of Netflix's catalog
- **Content growth over time** — a sharp increase in titles after 2015
- **Top 10 countries by content volume** — the United States leads by a wide margin
- **Rating distribution** — TV-MA and TV-14 are the most common ratings

## 💡 Key Insights

- Movies dominate the Netflix catalog over TV Shows
- Content production peaked after 2015
- The United States produces the largest share of content
- TV-14 is one of the most common content ratings
- The longest movie on the platform runs 312 minutes
- The longest-running TV Show has 16 seasons
- A small number of directors account for a disproportionately large share of titles

## ⚠️ Limitations

- Some records originally contained missing values, which were filled with `"Unknown"` rather than dropped in most cases, which may slightly affect distribution-based insights
- A title can belong to multiple genres, so genre-based counts may include overlap
- The dataset reflects Flixable's snapshot and may not match Netflix's current live catalog

## 🚀 How to Run

1. Clone this repository
2. Install dependencies:
```bash
   pip install pandas numpy matplotlib seaborn openpyxl
```
3. Open `Netflix_Data_Analysis.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab
4. Run all cells in order (make sure the dataset file is in the same directory, or update the file path in the first code cell)

## 📁 Repository Structure
