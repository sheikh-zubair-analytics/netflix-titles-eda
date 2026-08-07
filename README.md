# netflix-titles-eda
Exploratory data analysis of the Netflix titles catalog (2021) — examines content type mix, top producing countries, catalog growth over time, ratings, and genre trends using Python, Pandas, and Matplotlib/Seaborn.
# 🎥 Netflix Titles — Exploratory Data Analysis

Exploratory data analysis of the Netflix titles catalog (2021 snapshot) — examining content type mix, top content-producing countries, catalog growth over time, content ratings, and genre trends.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4c72b0)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Overview

Netflix is one of the largest global streaming platforms, and understanding its catalog composition reveals content strategy, regional investment patterns, and audience targeting. This project analyzes the Netflix titles dataset to answer key questions about the catalog's structure and growth.

**Objectives:**
- Understand the mix of Movies vs. TV Shows
- Identify the top content-producing countries
- Track how the catalog has grown over time
- Study the distribution of content ratings and genres
- Derive insights that support content strategy decisions

---

## 📂 Dataset

| Detail | Description |
|---|---|
| Source | Netflix Titles dataset (2021 snapshot) |
| Format | CSV |
| Rows / Columns | 8,807 titles × 12 columns |
| Key Fields | `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in`, `description` |

---

## 🛠️ Tools & Libraries

- **Python** — core language
- **Pandas** — data cleaning and manipulation
- **Matplotlib / Seaborn** — data visualization
- **Jupyter / Google Colab** — analysis environment

---

## 🔍 Project Workflow

1. **Data Collection** — load the Netflix titles dataset
2. **Data Cleaning & Preprocessing** — handle missing values in `director`, `cast`, `country`; parse `date_added` into a proper datetime; engineer a `year_added` feature
3. **Exploratory Data Analysis (EDA)** — examine distributions of type, country, rating, and genre
4. **Data Visualization** — count plots, bar charts, and line charts
5. **Insight Generation** — interpret charts to surface catalog trends
6. **Conclusion & Recommendations** — summarize findings for content strategy

---

## 📊 Key Findings

### 1. Movies vs. TV Shows
Movies make up roughly **70%** of the catalog vs. **30%** for TV Shows.

<img src="images/type_split.png" width="450"/>

### 2. Top Content-Producing Countries
The **United States** and **India** are the largest content sources by far.

<img src="images/top_countries.png" width="450"/>

### 3. Catalog Growth Over Time
Growth was flat before 2015, rose sharply from **2016–2019**, and dipped slightly in **2020–2021** (likely pandemic-related).

<img src="images/year_trend.png" width="450"/>

### 4. Content Ratings
**TV-MA** and **TV-14** are the most common ratings, indicating a mostly mature-audience catalog.

<img src="images/ratings.png" width="450"/>

### 5. Top Genres
"Dramas, International Movies," Documentaries, and Stand-Up Comedy lead the genre breakdown.

### 6. Movies vs. TV Shows — Growth Pattern
Both follow a similar growth curve, but Movie additions consistently outpace TV Show additions in volume.

<img src="images/movies_trend.png" width="420"/> <img src="images/tv_trend.png" width="420"/>

---

## 💡 Insights & Recommendations

- Continue investing in international drama, documentary, and stand-up comedy content given their proven volume
- Grow the TV Show pipeline to close the gap with Movie additions
- Improve metadata completeness, especially for `country` and `director` fields
- Monitor whether content additions recover to pre-2020 levels
- Maintain a mix of mature and family-oriented ratings to serve a broad subscriber base

---

## 📁 Repository Structure

```
netflix-titles-eda/
├── data/
│   └── netflix_titles_2021.csv
├── images/
│   ├── type_split.png
│   ├── top_countries.png
│   ├── year_trend.png
│   ├── ratings.png
│   ├── movies_trend.png
│   └── tv_trend.png
├── Netflix_EDA_Cleaned.ipynb
├── Netflix_Content_Analysis_Report.docx
└── README.md
```

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/<your-username>/netflix-titles-eda.git
cd netflix-titles-eda

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# Launch the notebook
jupyter notebook Netflix_EDA_Cleaned.ipynb
```

---

## 📄 License

This project is licensed under the MIT License — feel free to use and adapt it.

---

## 🙋 Author

Built as a data analysis & visualization project exploring the Netflix titles catalog.
