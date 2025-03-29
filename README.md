# 🌍 Access to Basic Services in Sub-Saharan Africa — SQL Project

Welcome to this data analysis project focused on **Access to Basic Services** (drinking water and sanitation) and **GDP** in **Sub-Saharan African countries**. This repository showcases how to use SQL **logic and comparison operators** to extract insights from the `united_nations.Access_to_Basic_Services` dataset using MySQL.

## 📚 Learning Objectives

This project is part of the ExploreAI Academy training and is designed to help learners:

- Understand how to use SQL `WHERE` clause and filtering logic
- Apply **logical and comparison operators** like:
  - `=`, `!=`, `<`, `>`, `<=`, `>=`
  - `AND`, `OR`, `NOT`
  - `IN`, `NOT IN`
  - `BETWEEN`
  - `IS NULL`, `IS NOT NULL`
- Perform **data analysis** to investigate potential relationships between GDP and access to basic services in Sub-Saharan Africa

---

## 🗃️ Dataset

The project uses the `Access_to_Basic_Services` table from the **`united_nations`** database.  
The key columns include:

- `Country_name`
- `Region`
- `Pct_managed_drinking_water_services`
- `Pct_managed_sanitation_services`
- `Est_gdp_in_billions`

---

## 💡 Key Questions Explored

- Is there a correlation between **GDP** and **access to drinking water** in Sub-Saharan Africa?
- Does a higher GDP correspond to **better sanitation services**?
- How do countries **not among the top five economies** in the region compare?

---

## 🧪 SQL Concepts Practiced

✅ Filtering using `WHERE`  
✅ Sorting using `ORDER BY` (`ASC`, `DESC`)  
✅ Using `IN`, `NOT IN`, `IS NULL`, `IS NOT NULL`  
✅ Logical conditions using `AND` / `OR`  
✅ Aggregating insights by country and region

---

## 🛠️ Requirements

To run this project locally, ensure you have:

- MySQL Workbench installed
- Access to the `united_nations` database
- A compatible SQL environment (e.g., MySQL Shell or local Jupyter with SQL connector)

**Note**: This project will not run on Google Colab due to local DB connection limitations.

---

## 🚀 How to Use

1. Clone the repository  
2. Open the SQL scripts in your preferred SQL editor  
3. Connect to your local MySQL instance  
4. Run queries to explore the dataset and answer key analysis questions

---

## 📊 Sample SQL Query

```sql
SELECT
    Country_name,
    Pct_managed_drinking_water_services,
    Est_gdp_in_billions
FROM
    access_to_basic_services
WHERE
    Region = 'Sub-Saharan Africa'
ORDER BY
    Pct_managed_drinking_water_services DESC;

```
## 📈 Insights & Observations
Some countries with higher GDP also show better access to basic services, but this is not consistent across all Sub-Saharan nations.

The rate of improvement in services does not always match GDP growth, indicating the need to explore governance, investment priorities, and infrastructure policies.

---

## 🙌 Acknowledgements
ExploreAI Academy for SQL training resources and dataset guidance

UN Data Repository for open access to global development datasets

---

## 🧑‍💻 Author
Ibrahim Ambale`
Data Analyst | Monitoring & Evaluation Specialist
Passionate about using data for development impact 🌱
