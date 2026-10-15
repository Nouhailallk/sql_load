# Data Analyst Job Market Analysis | SQL & PostgreSQL

## Project Overview

This project explores the Data Analyst job market through SQL analysis of job postings, salaries, and required technical skills. The goal is to better understand employer expectations, identify skills associated with higher salaries, and explore which technical skills are worth prioritizing for career development.

The project was completed as a hands-on learning exercise based on Luke Barousse's SQL tutorial, with a focus on practicing SQL queries and understanding how to translate data into useful insights.

## Business Questions

The analysis addresses five key questions:

1. Which Data Analyst positions offer the highest salaries?
2. What skills are required for the highest-paying positions?
3. Which technical skills appear most frequently in Data Analyst job postings?
4. Which skills are associated with higher average salaries?
5. Which skills offer a promising combination of demand and salary?

## Tools & Technologies

- **PostgreSQL** — querying and analyzing relational data.
- **SQL** — joins, aggregations, filtering, sorting, and Common Table Expressions (CTEs).
- **Visual Studio Code** — writing and executing SQL queries.
- **Git & GitHub** — version control and project documentation.

## Analysis Approach

### 1. Highest-Paying Data Analyst Jobs
Identified highly paid Data Analyst positions using salary filters and descending salary rankings to examine the opportunities available in the dataset.

SELECT job_id,
       job_title_short,
       job_location,
       job_schedule_type,
       salary_year_avg,
       job_posted_date,
       name AS company_name
FROM 
      job_postings_fact

LEFT JOIN company_dim ON job_postings_fact.company_id=company_dim.company_id
WHERE 
      salary_year_avg IS NOT NULL AND job_title_short='Data Analyst' AND job_location='Anywhere'
ORDER BY salary_year_avg DESC;

<img width="968" height="506" alt="image" src="https://github.com/user-attachments/assets/cb61620b-66b5-4e71-ac83-ec540f432449" />



### 2. Skills Required for High-Paying Roles
Combined job posting and skills data to identify the technical skills associated with the highest-paying positions.

### 3. Most In-Demand Skills
Counted skill occurrences across relevant job postings to identify the technologies most frequently requested by employers.

### 4. Skills and Average Salary
Compared average salaries across skills to explore the relationship between technical specialization and compensation.

### 5. Skills Prioritization
Combined skill demand and salary information to investigate which skills could be attractive priorities for aspiring Data Analysts.

## SQL Concepts Practiced

- JOIN operations across relational tables
- Aggregate functions such as COUNT() and AVG()
- GROUP BY and HAVING
- Common Table Expressions (CTEs)
- Filtering and sorting query results
- Data-driven analysis and interpretation

## Key Findings

The analysis examines salary differences between roles, recurring technical skill requirements, and the relationship between skill demand and compensation.

Specific findings and supporting figures will be documented here after reviewing the query results.

## Project Structure

```text
sql_load/
├── 1_create_database.sql
├── 1_Top_paying_jobs.sql
├── 2_Top_paying_skills.sql
├── 2_create_tables.sql
├── 3_Top_demanded_skills.sql
├── 3_modify_tables.sql
├── 4_Top_paying_skills.sql
└── 5_Most_optimal_skill.sql
```

*The filenames above reflect the scripts currently identified in the project; update this structure if your repository contains additional files or folders.*

## Learning Outcomes

This project provided practical experience in querying relational datasets, combining information from multiple tables, calculating analytical metrics, and investigating business questions using SQL.

It also strengthened my understanding of how job market data can support career research and skills prioritization.

## Acknowledgment

This project was completed as a guided learning exercise using the SQL tutorial by Luke Barousse. The analysis and documentation are presented as part of my own learning portfolio.

**Tutorial:** [Luke Barousse — SQL for Data Analytics](https://www.youtube.com/@LukeBarousse)
