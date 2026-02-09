# 📊 SQL Data Exploration Project
This project  focuses on exploring real-world data using **SQL**.  
The goal is to demonstrate practical SQL skills through data cleaning, exploration, and insight generation.

## 🔍 Project Purpose

This project shows my ability to:
- Work with real datasets  
- Import data into a SQL database  
- Write structured SQL queries  
- Analyze and explore data  
- Extract meaningful insights  
- Organize SQL code professionally  

---

## 🛠️ Tools & Technologies

- **SQL** (MySQL / SQL Server)
- **CSV Datasets**
- **GitHub** for version control
- *(Optional)* Excel for data preview

---

## 📁 Dataset Used

COVID-19 global dataset:

- `CovidDeaths.csv` – COVID deaths data  
- `CovidVaccinations.csv` – Vaccination data  

The datasets were imported into a SQL database for analysis.

---

## 📌 What This Project Does

✔ Imports raw data into SQL  
✔ Cleans and formats data  
✔ Explores data using SQL queries  
✔ Uses joins to combine datasets  
✔ Performs aggregations and filtering  
✔ Identifies patterns and trends  
✔ Produces meaningful insights  

---

## 🧠 Skills Demonstrated

- SQL querying  
- Data exploration  
- Data cleaning  
- Data analysis  
- Table joins  
- Aggregations (`SUM`, `COUNT`, `GROUP BY`)  
- Filtering (`WHERE`)  
- Sorting (`ORDER BY`)  
- Analytical thinking  
- Data interpretation  

---

## 🧪 Example SQL Queries

```sql
-- View data
SELECT *
FROM CovidDeaths;

-- Total deaths by country
SELECT country, SUM(deaths) AS total_deaths
FROM CovidDeaths
GROUP BY country
ORDER BY total_deaths DESC;

-- Join datasets
SELECT d.country, d.date, d.deaths, v.vaccinations
FROM CovidDeaths d
JOIN CovidVaccinations v
ON d.country = v.country AND d.date = v.date;

