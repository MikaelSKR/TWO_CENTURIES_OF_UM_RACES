# 🏃 Ultra-Marathon Race Analysis (USA, 2020) – 50K & 50Mi Insights

This is a self-directed tutorial project using Python to analyze performance trends in ultra-marathon races. The goal was to develop and showcase practical skills in **data cleaning**, **exploration**, and **visual storytelling**, while working with a large, real-world dataset from Kaggle.

Using Pandas and Seaborn, I focused on a filtered subset of ultra-marathon events — specifically **50-kilometer** and **50-mile** races in the **USA during 2020** — to explore performance differences by **gender**, **age group**, and **season**.

🔗 **Dataset Source**: [The Big Dataset of Ultra Marathon Running on Kaggle](https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running)

---

## 🧠 About the Dataset

According to Wikipedia, an **ultramarathon** is any race longer than the standard 42.195 km marathon distance. Common distances include **50K**, **100K**, **50 miles**, and **100 miles**, with some races extending beyond 200 miles. These events test the endurance and mental toughness of athletes worldwide.

The dataset contains:

- 🗓️ **7.4 million race records** (1798–2022)
- 👟 **1.6 million unique runners**
- 📍 Global events from public sources
- ✅ Anonymized data using unique `Athlete ID`s

Key columns include:

- Event name, date, and distance
- Athlete performance time
- Athlete gender and age
- Average speed (km/h)
- Number of finishers

---

## 📁 Dataset Access

Due to file size limitations, the full dataset is **not included** in this repo.  
Please download it manually from Kaggle:

🔗 [Download Dataset on Kaggle](https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running)

After downloading, place the dataset in the same folder as the Jupyter notebook to run the code.

---

## 🚀 Project Objectives

This tutorial project was built to explore and practice:

- 📊 Comparing **performance by gender** across 50K and 50Mi races
- 🎯 Identifying **best and worst performing age groups** in 50Mi races
- 🌦️ Investigating if **seasonal changes** affect average runner speed
- 🧹 Strengthening skills in data cleaning, transformation, and visualization

---

## 🛠️ Tools Used

- 🐍 Python (Jupyter Notebook)
- 🧮 Pandas for data wrangling
- 📊 Seaborn for data visualization
- 📁 Kaggle for dataset source

---

## 🔧 Workflow Summary

### 1. 📥 Load & Inspect
- Imported the dataset using Pandas
- Reviewed data types, columns, and null values

### 2. 🧹 Clean & Filter
- Filtered for:
  - Country: **USA**
  - Distance: **50K** or **50Mi**
  - Year: **2020**
- Cleaned up:
  - Event names (removed "(USA)")
  - Athlete performance times and speeds
  - Age column formatting
- Dropped unused columns (e.g., club, country, year of birth)
- Created new features like `season` based on race date

### 3. 📊 Analyze & Visualize
- Plotted speed distribution by gender
- Compared age groups (min 10–20 races) for performance rankings
- Visualized seasonal trends in average speed

---

## ❓ Questions Explored

1. 🧍‍♂️🧍‍♀️ How do **male and female runners** differ in average speed for 50K and 50Mi races?
2. 🎂 Which **age groups** perform best or worst in 50Mi races with at least 10 or 20 entries?
3. 🌦️ Does **season** (winter, spring, summer, fall) influence average running speed?

---

## 📈 Visuals

Created using `seaborn`:

- `sns.histplot()` – race length by gender  
- `sns.displot()` – speed distribution (50Mi)  
- `sns.violinplot()` – speed vs. gender for both distances  
- `sns.lmplot()` – age vs. speed regression by gender  

These charts helped communicate trends across gender, age, and seasonal splits clearly.

---

## 📎 Files in This Repo

- 📘 `TWO_CENTURIES_OF_UM_RACES.ipynb` – Jupyter notebook with all code and visualizations  
- 📝 `README.md` – This documentation

---

## 💡 Takeaways

This project gave me hands-on experience working with:

- A large, messy real-world dataset
- Data wrangling and feature engineering in Pandas
- Clear, accessible visual storytelling using Seaborn
- Deriving insights from filtered subsets of data

It’s a strong step toward applying data analysis skills to practical questions, and I look forward to building more projects like this.

---

## 📬 Contact

I'm actively building my portfolio and seeking opportunities in **data analysis** and **data storytelling** roles.  
If this work resonates with you or your team, feel free to reach out!

