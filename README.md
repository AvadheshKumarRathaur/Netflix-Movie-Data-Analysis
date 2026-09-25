# 🎬 Netflix Movie Data Analysis

An end-to-end **Data Analysis / EDA project** using Python to explore movie genres, ratings, popularity and release-year trends.

> **Note:** The supplied dataset is a movie dataset (`mymoviedb.csv`). Although this project is presented as a Netflix/movie analysis project, the dataset itself should not be treated as direct Netflix viewing or subscriber behavior data.

## 📌 Project Overview

This project covers:

- Data loading and inspection
- Data cleaning and preprocessing
- Missing-value and duplicate checks
- Date conversion and release-year extraction
- Vote-average categorization
- Multi-genre splitting and exploding
- Exploratory Data Analysis (EDA)
- Data visualization
- Key analytical questions
- Additional genre-level analysis
- Conclusions and limitations

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📂 Project Structure

```text
netflix-movie-data-analysis/
│
├── Netflix_Data_Analysis.ipynb
├── mymoviedb.csv
├── requirements.txt
├── README.md
└── .gitignore
```

## 🔎 Analysis Questions

1. What is the most frequent genre in the dataset?
2. What genres has highest votes ?
3. What movie got the highest popularity ? what's its genre ?
4. What movie got the lowest popularity ? what's its genre ?
5. Which year has the most filmmed movies?


## 🧹 Data Preparation

The notebook:

- Converts `Release_Date` into a datetime field.
- Extracts `Release_Year`.
- Removes `Overview`, `Original_Language`, and `Poster_Url` because they are not required for the planned analysis.
- Removes rows missing important analysis fields.
- Categorizes `Vote_Average` into four quartile-based groups.
- Splits comma-separated genres and explodes them into separate rows.

## 📊 Visualizations

The project includes visualizations for:

- Genre distribution
- Vote-average categories
- Movies by release year
- Average popularity by genre
- Average rating by genre

## 💡 Key Insights

The original analysis found that:

- **Drama** is the most frequent genre in the dataset.
- A substantial portion of the dataset falls into the `popular` vote category after quartile-based categorization.
- **Spider-Man: No Way Home** has the highest popularity value in the supplied dataset.
- The original notebook identifies **2020** as the year with the highest number of movies.
- Genre-level analysis can reveal differences in average popularity and ratings.

Because the cleaned notebook recalculates these values directly from the supplied CSV, run the notebook to reproduce the exact current outputs.

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/AvadheshKumarRathaur/Netflix-Movie-Data-Analysis.git
cd netflix-movie-data-analysis
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Netflix Data Analysis.ipynb
```

## 📈 Dataset

File: `mymoviedb.csv`

The dataset contains movie-level information such as:

- Release Date
- Title
- Popularity
- Vote Count
- Vote Average
- Genre
- Original Language
- Overview
- Poster URL

## ⚠️ Dataset Limitation

This dataset contains movie metadata and popularity/rating information. It does **not** by itself provide Netflix watch history, subscriber behavior, viewing hours, or recommendation outcomes. Therefore, conclusions should be described as findings from the supplied movie dataset rather than direct Netflix customer analytics.


## 👨‍💻 Author

**Avadhesh Kumar Rathaur**

B.Tech Computer Science | Data Analytics & Python

---
⭐ If you find this project useful, consider giving the repository a star!
