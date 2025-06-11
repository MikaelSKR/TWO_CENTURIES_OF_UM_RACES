# 🏃 Ultra-Marathon Race Analysis (USA, 2020) – 50K & 50Mi Insights

This project explores performance trends in ultra-marathon races using data science techniques in Python. By focusing on 50-kilometer and 50-mile races held in the United States in 2020, I aimed to uncover insights related to **gender performance**, **age group effectiveness**, and **seasonal impact on athlete speed**.

🔗 **Dataset Source**: [The Big Dataset of Ultra Marathon Running on Kaggle](https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running)

---

## 🚀 Project Goals

- 🎯 Understand performance differences between **male and female runners**
- 📊 Identify **top and bottom-performing age groups** in 50-mile races
- 🌦️ Analyze if **seasonal changes** (e.g., summer vs. winter) affect athlete speed
- 🧠 Practice data cleaning, feature engineering, and visual storytelling

---

## 📁 Dataset Focus

From a large global dataset, I filtered the data down to:
- 🇺🇸 **USA-only** races  
- 🏁 **50K or 50Mi** distances  
- 📅 **Year 2020**

I also identified two races I personally ran in: **Sarasota** and **Everglades**, adding a personal layer to the analysis.

---

## 🔧 Process Overview

### 1. 📥 Data Import & Initial Exploration
- Loaded the dataset using Pandas
- Previewed structure, columns, data types, and null values

### 2. 🧹 Data Cleaning & Filtering
- Filtered by:
  - `event_country == 'USA'`
  - `race_length == '50km' or '50mi'`
  - `event_year == 2020`
- Removed “(USA)” from event names
- Cleaned time and speed data for numeric analysis
- Dropped unnecessary columns like athlete club, country, birth year
- Checked for nulls, duplicates, and reset the index

### 3. 🧠 Feature Engineering
- Created a `season` column based on race month:
  - Winter: Dec–Feb
  - Spring: Mar–May
  - Summer: Jun–Aug
  - Fall: Sep–Nov
- Cleaned and cast columns for analysis (e.g. float conversion of speed, performance time)
- Renamed columns to snake_case for consistency

---

## 🔍 Key Questions Answered

1. **Who’s faster: men or women in 50k/50mi races?**
2. **What are the top 15 age groups in 50mi races (20+ races)?**
3. **What are the bottom 20 age groups in 50mi races (10+ races)?**
4. **Is athlete speed lower in summer vs. winter?**

---

## 📊 Visualizations & Methods

Used **Seaborn** and **Matplotlib** to explore trends through:

- `sns.histplot()` for gender vs distance distributions  
- `sns.displot()` to show speed distributions in 50mi races  
- `sns.violinplot()` for gender-based speed spreads in both race types  
- `sns.lmplot()` for regression of age vs speed by gender  
- Custom grouping and aggregation logic for age group performance  
- Seasonal comparisons with bar plots for average speeds  

---

## 📈 Tools Used

- 🐍 **Python (Jupyter Notebook)**
- 🧮 **Pandas** – for cleaning, filtering, calculations
- 📉 **Seaborn** – for visualization
- 💬 Markdown – for clean documentation and storytelling

---

## 🏁 Personal Note

This project blends technical analysis with personal context — having run two of the races in the dataset made the process even more rewarding. It demonstrates how data analysis can provide meaningful narratives beyond just numbers.

---

## 🔗 Project Files

- 📘 `TWO_CENTURIES_OF_UM_RACES.ipynb` – Full notebook with code and analysis  
- 🗎 `TWO_CENTURIES_OF_UM_RACES.csv` – CSV version RAW Dataset 

---

## 📬 Let’s Connect

If you're a recruiter or fellow data enthusiast looking for collaborative talent, feel free to reach out. I'm actively exploring roles in **data analysis** or **data storytelling** using Python.

