# Pandas Data Analysis

Daily practice of data analysis using **Pandas**, **Matplotlib** and **Seaborn**. Each project is in its own folder with the notebook and dataset.

## Table of Contents

1. [Adult Income Analysis](#1-adult-income-analysis)
2. [Google Play Store Data Analysis](#2-google-play-store-data-analysis)
3. [YouTube Channel Data Analysis](#3-youtube-channel-data-analysis)

---

## 1. Adult Income Analysis

**Folder:** [`adult-income-analysis/`](adult-income-analysis/)
**Dataset:** [Adult Census Income (Kaggle)](https://www.kaggle.com/datasets/uciml/adult-census-income)

### About
Exploratory data analysis on the Adult Census Income dataset. The dataset has details like age, workclass, education, marital status, occupation, gender, hours per week and income. The goal is to find which factors affect whether a person earns `<=50K` or `>50K`.

### What I did
- Loaded the CSV file and checked its structure.
- Looked at the columns, unique values and value counts of the `income` column.
- Encoded the `income` column into numbers (0 and 1) using `apply()` and a custom function.
- Found which workclass has the highest share of `>50K` earners using `groupby()`.
- Compared the chance of earning `>50K` between Male and Female.
- Converted the `workclass` column to the `category` datatype to save memory.
- Did univariate and bivariate analysis with plots.

### Concepts Covered
`read_csv`, `columns`, `unique`, `value_counts`, `apply`, `replace`, `groupby`, `sort_values`, `astype`, `info`, `countplot`, `boxplot`

---

## 2. Google Play Store Data Analysis

**Folder:** [`google-playstore-data-analysis/`](google-playstore-data-analysis/)
**Dataset:** [Google Play Store Apps (Kaggle)](https://www.kaggle.com/datasets/lava18/google-play-store-apps)

### About
Analysis of apps on the Google Play Store. The dataset contains the app name, category, rating, reviews, size, installs, type (free or paid), price and more. The goal is to understand app ratings, reviews and installs across categories.

### What I did
- Viewed the first and last rows, and checked shape, info and overall statistics.
- Counted the apps whose title contains a keyword (for example "Astrology").
- Found the average app rating and the number of unique categories.
- Found the category with the highest average rating.
- Counted apps with a 5-star rating.
- Cleaned the `Reviews` column (fixed the `3.0M` value and converted it to float) and found the average reviews.
- Counted free and paid apps and compared their average ratings.
- Found the app with the most reviews and the top 5 apps by reviews.
- Cleaned the `Installs` column (removed `,` and `+`, fixed the `Free` value) and found the top 5 apps by installs.

### Concepts Covered
`head`, `tail`, `shape`, `info`, `describe`, `str.contains`, `mean`, `nunique`, `groupby`, `value_counts`, `replace`, `astype`, `str.replace`, `sort_values`, `iloc`

---

## 3. YouTube Channel Data Analysis

**Folder:** [`youtube-channel-data-analysis/`](youtube-channel-data-analysis/)
**Dataset:** [Top 5000 YouTube Channels (Kaggle)](https://www.kaggle.com/datasets/themlphdstudent/top-5000-youtube-channels-data-from-socialblade)

### About
Analysis of the top 5000 YouTube channels. The dataset contains the channel rank, grade, video uploads, subscribers and total video views. The goal is to clean messy data and find which grade of channels performs best.

### What I did
- Displayed rows using `head(-5)` and `tail(-5)`, and checked shape, info and statistics.
- Replaced the `--` values with `NaN` and checked missing values with a heatmap.
- Dropped the rows with missing values.
- Cleaned the `Rank` column (removed extra characters and commas, converted to int).
- Converted `Video Uploads` and `Subscribers` to int.
- Mapped the `Grade` column to numbers (`A++` = 5, `A+` = 4, `A` = 3, `A-` = 2, `B+` = 1).
- Created a new column `Avg_views` (video views divided by video uploads).
- Found the top 5 channels by video uploads.
- Found the correlation matrix of the numeric columns.
- Compared grades by video uploads, average views and subscribers using bar plots.
- Found which grade has the highest video views using `groupby`.

### Concepts Covered
`head`, `tail`, `info`, `describe`, `replace`, `isnull`, `dropna`, `heatmap`, `str` methods, `astype`, `map`, new column creation, `sort_values`, `corr`, `barplot`, `groupby`

---

## Tools Used

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## How to Run

1. Clone the repository:
   ```
   git clone https://github.com/your-username/pandas-data-analysis.git
   ```
2. Install the libraries:
   ```
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Open Jupyter Notebook:
   ```
   jupyter notebook
   ```
4. Open any project folder and run the `.ipynb` file.


---

New projects will be added regularly.
