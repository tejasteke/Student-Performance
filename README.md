#  Student Performance Dashboard (Power BI)

An interactive Power BI dashboard that explores how factors such as **parental education, lunch type, race/ethnicity group, gender and test preparation** relate to students' exam performance in **Math, Reading and Writing**.



---

##  Project Overview

The goal of this project is to analyze student exam scores and find out which background factors are associated with higher academic performance. The data was cleaned and transformed, a combined score column was created, and the results were visualized in a single-page Power BI dashboard with slicers for filtering.

---

## Tools & Technologies

- **Power BI Desktop** – data cleaning, modeling, DAX and visualization
- **Power Query** – data transformation and value replacement
- **Excel / CSV** – source data

---

##  Data Cleaning & Preparation

- **Replaced values in the Parental Level of Education column** to standardize the education categories used in the analysis
- **Created a new column `Percentage`** by combining the three subject scores to get an overall performance measure:

  ```
  Percentage = (Math Score + Reading Score + Writing Score) / 3
  ```
- Used this `Percentage` column to compare overall performance across groups
- Checked data types and column names for consistency before building visuals

---

##  Dashboard Features

| Visual | Purpose |
|---|---|
| **KPI cards** | Average Math, Reading and Writing scores |
| **Average Percentage by Lunch** | Compare standard vs free/reduced lunch |
| **Average Percentage by Parental Level of Education** | See how parent education relates to performance |
| **Average Percentage by Race/Ethnicity and Lunch** | Compare groups A–E split by lunch type |
| **Average Percentage by Race/Ethnicity and Parental Education** | Stacked view of group and parental education |
| **Average Percentage by Gender** | Overall performance by gender |
| **Reading & Writing Score by Gender** | Line chart comparing gender in language subjects |
| **Slicers** | Filter by Test Preparation Course and Gender |

### Headline KPIs

| Subject | Average Score |
|---|---|
| Math | 66.09 |
| Reading | 69.17 |
| Writing | 68.05 |

---

##  Key Insights

### 1. Parental education is associated with student performance
Students whose parents have a higher level of education tend to score higher.

| Parental Level of Education | Avg. Percentage |
|---|---|
| Master's degree | 73.95 |
| Bachelor's degree | 72.22 |
| Associate's degree | 69.91 |
| Some college | 68.83 |
| High school | 64.38 |

### 2. Lunch type shows a socioeconomic pattern
Students with a **standard lunch (71.17)** score higher on average than students with a **free/reduced lunch (62.54)**.

Lunch itself does not affect studying. It is most likely a **proxy for family income**: students who can afford a standard lunch probably come from better-off households. This suggests that **standard of living and economic background are linked to academic performance**. The same gap appears in every race/ethnicity group (A to E).

### 3. Group E has the highest average performance
Group E has the highest average percentage compared with the other groups. This holds for both lunch types (Group E: 67.90 free/reduced, 75.24 standard).

### 4. Gender differences by subject
- **Female** students score higher in **Reading and Writing** (about 72.5 on average, vs roughly 63 to 65 for male students)
- **Male** students score higher in **Math**

### 5. Test preparation helps
| Test Preparation Course | Avg. Score |
|---|---|
| Completed | **69.70** |
| None | **64.08** |

Students who completed the preparation course scored about **5.6 points higher** on average.

---

##  Note on Interpretation

These findings show **associations, not proven causes**. For example, lunch type is used as an indirect indicator of economic background, because the dataset has no income column. Group labels (A–E) are anonymized, so the reason behind group differences cannot be determined from this data alone.

---



---


##  Author

**Tejas**
MCA Student | Aspiring Data Analyst
Skills: Python, SQL, Power BI, Excel

🌐 Portfolio: [tejasteke.github.io](https://tejasteke.github.io)

---

⭐ If you found this project useful, consider giving the repo a star!
