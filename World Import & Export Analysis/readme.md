![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Data Analytics](https://img.shields.io/badge/Data_Analytics-0047AB?style=for-the-badge)

#  World Import & Export Analysis with MySQL

## Exploring 34 Years of Global Trade Through SQL  
*Transforming raw import and export records into meaningful business insights.*

---

##  Skills
`MySQL` • `Data Analysis` • `Filtering` • `Pattern Matching` • `Sorting` • `Query Optimization`

---

## Overview

Data is only valuable when it answers questions.

This project explores a **34-year world import and export dataset** using MySQL to uncover trends, identify top trading regions, and practice writing efficient SQL queries.

Instead of simply demonstrating SQL syntax, the goal is to simulate how a real analyst approaches data:

> What patterns exist? Which regions dominate global trade? How can SQL transform thousands of rows into actionable insights?

Every query in this repository is written with those questions in mind.

---

## Why This Project?

I chose this project because I was curious about which economies have the most trade volume.I wanted to move beyond commands like this to actuallya answering questions:

```sql
SELECT * FROM table;

Instead of just learning SQL syntax, this project focuses on asking real analytical questions that matter to business and data teams.

Working with international trade data helped me practice:

- Extracting meaningful insights from large datasets  
- Filtering relevant records  
- Ranking results based on business metrics  
- Writing clean and maintainable SQL  

This project is part of my journey toward becoming a **data analyst** who can confidently work with databases.

---

## Skills Demonstrated

### Database Operations
- Creating and managing schemas  
- Importing structured datasets into MySQL  
- Working with MySQL Workbench  

### SQL Querying
- `SELECT`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `LIKE`
- Column aliasing  

### Analytical Thinking
- Filtering datasets based on conditions  
- Ranking trading partners by export performance  
- Comparing imports and exports across years  
- Extracting insights from raw data  

---

## Dataset

The dataset contains **34 years of global trade data**, including:

| Column | Description |
|--------|-------------|
| Partner Name | Trading partner or region |
| Year | Trade year |
| Export (US$ Thousand) | Total exports |
| Import (US$ Thousand) | Total imports |

This structure provides strong opportunities for exploratory data analysis.

---

## Example Analysis

### Question ?
Which trading partners beginning with **"E"** recorded the highest export values?

```sql
SELECT
    `partner name`,
    `year`,
    `export (US$ Thousand)`,
    `import (US$ Thousand)`
FROM world_import_export.`34_years_world_export_import_dataset`
WHERE `partner name` LIKE 'E%'
ORDER BY `export (US$ Thousand)` DESC
LIMIT 15;

## Key Insights

By combining **filtering, sorting, and limiting**, the analysis identifies top-performing exporting regions that match specific conditions.

This demonstrates how even simple SQL operations can produce meaningful insights when applied correctly to real datasets.

---

## What I Learned

This project reinforced that **SQL is not just a query language — it is an analytical tool for decision-making.**

Through this analysis, I developed stronger skills in:

- Identifying patterns hidden within large datasets  
- Validating assumptions using structured queries  
- Supporting data-driven decision-making  
- Translating raw data into meaningful insights  
- Thinking like a data analyst, not just a SQL user  

Most importantly, it strengthened my ability to approach data with curiosity and structure rather than just syntax.

---

## Future Improvements

To further enhance this analysis, the following improvements are planned:

- [ ] Advanced aggregations using `SUM()`, `AVG()`, `COUNT()`  
- [ ] `GROUP BY` and `HAVING` for deeper segmentation analysis  
- [ ] Window functions for ranking and trend analysis  
- [ ] Creation of views and stored procedures for reusable logic  
- [ ] Integration with **Power BI** or **Python (Pandas/Matplotlib)** for visualization  
- [ ] Query performance optimization using indexing strategies  

---

## Final Thoughts

Every dataset tells a story — the key is knowing how to ask the right questions.

This journey through **34 years of global trade data** has reinforced that technical proficiency is only one part of the equation. The other, equally important part, is curiosity — the ability to explore, question, and look beyond the numbers.

Working through this project strengthened my understanding that real insight comes not just from writing queries, but from thinking critically about what the data represents and why it matters.

---

## Continuous Growth

I am constantly looking for the next dataset to explore and the next problem to solve. Each project is an opportunity to improve my analytical thinking, refine my SQL skills, and deepen my understanding of real-world data systems.

---

## Let’s Connect

If you have suggestions for datasets, feedback on my query structure,feel free to reach out or connect.



__ Continuous learning is the goal — every dataset is a new opportunity to grow.
