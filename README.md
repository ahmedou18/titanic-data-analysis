# Titanic Dataset - Exploratory Data Analysis (EDA)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Latest-orange.svg)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Latest-teal.svg)](https://seaborn.pydata.org/)

An end-to-end Exploratory Data Analysis (EDA) on the historic Titanic dataset using Python. This project highlights crucial data science workflows, including **data cleaning, missing value imputation, and advanced data visualization** to uncover the socio-demographic factors that influenced survival rates.

---

## 📌 Project Overview
The objective of this project is to analyze the passenger manifesto of the RMS Titanic and answer the fundamental question: **"Who were the passengers who survived, and what factors played a role in their survival?"**

### Key Technical Skills Demonstrated:
* **Dynamic Data Ingestion:** Importing data directly via remote URLs.
* **Data Cleaning & Preprocessing:** Identifying and strategically handling missing values (e.g., age imputation).
* **Statistical Analysis:** Avoiding the "trap of averages" by exploring multi-variable relationships.
* **Data Storytelling & Visualization:** Translating statistical outputs into logical, human stories using `Seaborn` and `Matplotlib`.

---

## ❓ The 5 Core Analytical Questions
To structure the analysis, the project deep-dives into five primary hypotheses:
1. **Global Survival Rate:** What was the overall survival baseline on the ship?
2. **Gender Influence:** Did the traditional "Women and children first" maritime protocol hold true?
3. **Socio-Economic Status (Social Class):** Did ticket class and fare affect evacuation priority?
4. **Age Demographics:** What role did age play, and how do missing values impact our understanding of the metrics?
5. **Family Dynamics:** Was it safer to travel solo or accompanied by family members?

---

## 📊 Key Insights & Analytics Summary

### 1. Overall Survival Rate
* **Deceased (0):** 61.62%  
* **Survived (1):** 38.38%  
* *Insight:* The tragedy was devastatingly massive, with fewer than 4 out of 10 passengers making it out alive, primarily due to the severe lack of lifeboats.

### 2. Gender: The Single Most Determinant Factor
* **Females:** 74.20% Survival Rate  
* **Males:** 18.89% Survival Rate  
* *Insight:* Chivalric protocols were strictly enforced; a female passenger was nearly 4 times more likely to survive than a male passenger.

### 3. Social Class: Socio-Economic Inequality
* **1st Class:** 62.96% | **2nd Class:** 47.28% | **3rd Class:** 24.24%  
* *Insight:* Survival was heavily stratified. 1st-class passengers had a distinct advantage, likely due to cabin locations being closer to the upper decks and better access to lifeboats.

### 4. Age: The Trap of Averages & The Reality of Sacrifice
* **Average Age (Raw Data):** Deceased: 30.63 yrs | Survived: 28.34 yrs  
* **Average Age (After Imputation):** Deceased: 30.03 yrs | Survived: 28.29 yrs  
* *Insight:* Looking only at the mean suggests age didn't matter. However, **Kernel Density Estimate (KDE) visualizations** reveal a massive spike in survival for children (0-10 years), proving they were prioritized, while young adult males sacrificed their places. Imputing the missing values smoothed the data, bringing the statistical means closer while solidifying this moral narrative.

### 5. Family Size: The Sweet Spot of Survival
* **Solo Travelers:** 30.35% Survival Rate  
* **Small Families (2–4 members):** Up to 72.41% Survival Rate  
* **Large Families (5+ members):** Survival rates dropped drastically, hitting 0% for very large families.  
* *Insight:* Traveling alone was a handicap (no support network), but traveling in overly large families was fatal due to the extreme difficulty of regrouping a large group amidst chaos and darkness.

---

## 🛠️ Technologies & Libraries Used
* **Environment:** Google Colab / Jupyter Notebooks
* **Language:** Python 3
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `seaborn`, `matplotlib`

---

## 🚀 How to Run This Project
Since the dataset is fetched dynamically from a public GitHub repository, you do not need to download any external CSV files.

1. Clone this repository:
   ```bash
   git clone [https://github.com/ahmedou18/titanic-data-analysis.git](https://github.com/ahmedou18/titanic-data-analysis.git)

2. Open the .ipynb file in Google Colab or Jupyter Notebook.

3. Run all cells sequentially to generate the data frames, statistical summaries, and interactive plots.


## 📬 Contact
Created by **Ahmedou Mohamed Lemine** - feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/ahmedou-mohamed-lemine-84923824a?utm_source=share_via&utm_content=profile&utm_medium=member_android) or check out my other data science projects!