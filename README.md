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

<img width="968" height="506" alt="image" src="https://github.com/user-attachments/assets/cb61620b-66b5-4e71-ac83-ec540f432449" />


### 2. Skills Required for High-Paying Roles
Combined job posting and skills data to identify the technical skills associated with the highest-paying positions.
 
<img width="1046" height="767" alt="image" src="https://github.com/user-attachments/assets/913bf525-8637-4ea2-a86b-98107a478d77" />

### 3. Most In-Demand Skills
Counted skill occurrences across relevant job postings to identify the technologies most frequently requested by employers.

<img width="296" height="292" alt="image" src="https://github.com/user-attachments/assets/1b16a9ae-8341-4ed9-9744-9b1ef66fdafb" />

### 4. Skills and Average Salary
Compared average salaries across skills to explore the relationship between technical specialization and compensation.

<img width="300" height="316" alt="image" src="https://github.com/user-attachments/assets/31390771-f066-403d-acf4-f461651aca6c" />

### 5. Skills Prioritization
Combined skill demand and salary information to investigate which skills could be attractive priorities for aspiring Data Analysts.

<img width="594" height="305" alt="image" src="https://github.com/user-attachments/assets/dd74e587-a3e7-45fb-9a92-4323cf0f0a6b" />

## SQL Concepts Practiced

- JOIN operations across relational tables
- Aggregate functions such as COUNT() and AVG()
- GROUP BY and HAVING
- Common Table Expressions (CTEs)
- Filtering and sorting query results
- Data-driven analysis and interpretation

## Key Findings

1. Highest-Paying Data Analyst Jobs

Identified high-paying remote Data Analyst opportunities, with annual salary estimates reaching $650,000 in the dataset.

Mantys ranked first, followed by Meta at $336,500 and AT&T at $255,829.50.

2. Skills Required for High-Paying Jobs

Analyzed the skills associated with high-paying Data Analyst positions to identify technical requirements for well-compensated roles.

The AT&T position, with an estimated annual salary of $255,829.50, lists a broad technical stack, including SQL, Python, R, Azure, Databricks, AWS, Pandas, PySpark, Jupyter, Excel, Tableau, Power BI, and PowerPoint.

Other high-paying opportunities in the results include positions at Pinterest Job Advertisements ($232,423) and Uclahealthcareers ($217,000).

These results highlight the combination of programming, cloud platforms, data processing, and visualization tools that may be relevant to high-paying Data Analyst roles.

3. Most In-Demand Skills

The most frequently requested skills for Data Analyst positions in the dataset were:SQL ranked first, followed by Excel and Python.

Tableau and Power BI also appeared frequently, highlighting the importance of data visualization alongside querying and analysis.

4. Skills and Average Salary

Compared average annual salaries across skills to explore compensation differences.

SVN ranked first in the displayed results at $400,000, followed by Solidity at $179,000 and Couchbase at $160,515.

These results should be interpreted carefully: some skills may appear in relatively few job postings, and the displayed averages do not establish that a skill alone causes higher pay.

5. Optimal Skills for Career Development

Combined skill demand and average salary to identify potentially valuable skills for Data Analysts.

SQL appeared in 398 job postings in the displayed results, with an average salary of $97,237.

Python appeared in 236 postings, with an average salary of $101,397.

Power BI appeared in 110 postings, with an average salary of $97,431.

These findings suggest that SQL, Python, and Power BI are worth prioritizing when balancing employer demand with salary potential.

Conclusion

The analysis highlights SQL, Excel, Python, Tableau, and Power BI as frequently requested Data Analyst skills. Combining strong SQL fundamentals with Python and Power BI can help candidates develop a skill set aligned with many roles in the dataset. Salary comparisons should also account for job requirements, experience, and the number of observations behind each average.

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
