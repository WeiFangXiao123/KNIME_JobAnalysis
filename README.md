# KNIME_JobAnalysis
<img width="923" alt="Screenshot 2025-06-02 at 5 12 05 PM" src="https://github.com/user-attachments/assets/e7834012-6ef7-44c6-b1dd-cb294ebca20a" />

# Storyline
This analysis explores what makes Senior Data Analyst roles competitive in today’s job market. By examining job postings across companies, locations, platforms, and salary ranges, we aim to understand the key factors influencing job visibility and desirability in the tech industry.

# How KNIME Nodes Were Used
The entire analysis was performed using a structured workflow in KNIME. Each node played a specific role in helping clean, transform, and analyze the Yelp data:
- **DB Table Selector:** Used to select the table from the connected SQL database.
- **DB Column Filter/ Column Filter:** Removed unnecessary columns, keeping only the relevant features such as company, title, via, etc.
- **DB Row Filter/ Row Filter:** Kept only the titles equal to “Senior Data Analyst”, which is the main target that we want to analyze.
- **DB reader:** Run the input query on the database and loads the results into a KNIME data table.
- **GroupBy:** Aggregated the data by individual restaurant categories and calculated the number of hiring posts, positions, and remote work opportunities.
- **Sorter:** Sorted the grouped data in descending order to find top 5 Senior Data Analyst hiring companies.
- **Top k Row Filter:** Selected the top 5 Senior Data Analyst hiring companies.
- **Bar Chart:** Visualized top 5 Senior Data Analyst hiring companies and Senior Data Analysts maximum salary by companies.
- **Pie Chart:** Visualized remote work availability for senior data analyst roles and distribution of senior data analyst listings across job platforms.
- **Table View:** Created a table for understanding how many senior data analysts each company is hiring.

# Bar Chart – Senior Data Analyst Maximum Salary by Companies
![Bar Chart](https://github.com/user-attachments/assets/05092e91-84b4-4746-aff9-0f63a22c8121)

**Purpose:**
To reveal which companies offer the highest maximum salaries for the same role.
This highlights potential employers with strong compensation packages, helping job seekers prioritize opportunities and helping companies benchmark their offers.

**Insight Example:**
If certain companies consistently appear with higher maximum salaries, they may be more competitive or require niche expertise.

# Pie Chart – Remote Work Availability for Senior Data Analyst Roles
![Pie Chart](https://github.com/user-attachments/assets/3690535f-ca6f-4a25-a13e-e4e24b7fd0cc)

**Purpose:**
To compare how many job postings for Senior Data Analyst roles offer **remote options** versus those that do not specify or are in-office. This reflects how flexible the tech job market is for this position, important for understanding the evolving work culture.

**Insight Example:**
If certain companies consistently appear with higher maximum salaries, they may be more competitive or require niche expertise.

# Pie Chart – Distribution of Senior Data Analyst Listings Across Job Platforms
![Pie Chart2](https://github.com/user-attachments/assets/5a51048c-bc6c-4752-b667-dabcd00c05be)

**Purpose:**
To identify which job posting platforms (e.g., LinkedIn, Indeed) are most commonly used by companies hiring Senior Data Analysts. This is useful for both job seekers and recruiters.

**Insight Example:**
If LinkedIn dominates, it suggests higher traction and visibility for tech roles on that platform.

# Bar Chart – Top 5 Senior Data Analyst Hiring Companies
![Bar Chart2](https://github.com/user-attachments/assets/cbeb22ee-775f-40da-9ea0-efe36db1ff47)
**Purpose:**
To spotlight the top 5 employers by number of job postings. This visually summarizes the table data and emphasizes key players in the hiring market.

**Insight Example:**
The top 5 companies can be considered the most aggressive or active in hiring for this role.

# Conclusion
Together, these outputs paint a complete picture of the Senior Data Analyst job market, including salary competitiveness, hiring trends, remote work availability, and recruiting channels. This provides valuable guidance to job seekers, recruiters, and HR strategists.



