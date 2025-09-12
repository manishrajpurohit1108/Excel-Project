# 📊HR Attrition Analysis (Excel Project)

## 📝 Project Title  
**HR Attrition Analysis Dashboard**


**Short description:** Interactive Excel dashboard and analysis to understand drivers of employee attrition (age, department, salary, tenure, city, location) and recommend retention actions.

---

## 🎯 Project Objectives
- Analyze employee attrition patterns to identify key drivers of turnover.  
- Understand how factors such as **age, gender, department, salary, tenure, and city** influence attrition.  
- Build an **interactive Excel dashboard** with KPIs, slicers, and visuals for HR teams.  
- Provide insights that can help organizations improve **employee retention strategies**.  

---

## 📂 Dataset Details  
- **Dataset Name:** HR Attrition Indian Dataset  
- **Source:** [Dataset](https://github.com/manishrajpurohit1108/Excel-Project/blob/main/HR_Attrition_Indian_Dataset.csv) from Kaggle
- **Columns (22 total):**  

  - **FullName** → Synthetic full name of the employee  
  - **Age** → Age of the employee in years  
  - **Gender** → Gender identity of the employee  
  - **Department** → Department in which the employee is currently working  
  - **Designation** → Employee's current job title or role  
  - **EducationQualification** → Highest educational qualification completed  
  - **MonthlySalary** → Monthly salary of the employee (in Indian Rupees)  
  - **DateOfJoining** → Date the employee joined the company  
  - **YearsWithCompany** → Total number of years the employee has worked with the company  
  - **YearsInRole** → Number of years the employee has spent in their current role  
  - **AppraisalRating** → Performance appraisal rating (1 = Poor to 5 = Excellent)  
  - **TrainingHours** → Total training hours completed in the last financial year  
  - **DoesOvertime** → Whether the employee frequently works overtime (Yes/No)  
  - **JobSatisfaction** → Self-reported job satisfaction level (1 = Low to 5 = High)  
  - **WorkLifeBalance** → Self-assessed work-life balance (1 = Poor to 4 = Excellent)  
  - **MaritalStatus** → Marital status of the employee  
  - **PreviousCompanies** → Number of companies the employee worked at before the current one  
  - **DistanceFromHome** → Distance from employee’s residence to the office (in kilometers)  
  - **LeavesTaken** → Number of leave days taken in the last calendar year  
  - **City** → City in India where the employee’s office is located  
  - **LeftCompany** → Target column – Whether the employee has left the company (Yes/No)

---

## 🛠️ Steps / Process Followed

1. **Dataset Preparation**
   - Loaded the dataset (5,000 records) into Excel using Power Query’s Get Data option.
   - Checked for duplicates and null values, none found.   
   - Ensured date formats and numeric types were correct.

2. **Additional columns created (in Power Pivot)**
   - `AgeGroup` (`<25`, `25–35`, `36–45`, `46+`).  
   - `SalaryBracket` (`<25K`, `25K–50K`, `50K–75K`, `75K+`).  
   - `TenureCategory` (`<1 Year`, `1–3 Years`, `4–5 Years`, `5+ Years`).  
   - `WorkLifeBalanceCategory` (mapped as `Poor`, `Good`, `Fair` and `Excellent` according to numeric 1–4 to labels).  
   - `JobSatisfactionCategory` (mapped as `Very Low`, `Low`, `Medium`, `High` and `Very High` according to numeric 1–5 to labels).  
   - `DistanceFromHomeCategory` grouped as: `0–5 km`, `6–15 km`, `16–30 km`, `30+ km`.

3. **KPIs Built (PivotTable)**
   - **Total Employees**  
   - **Active Employees**  
   - **Attrition Count**  
   - **Attrition Rate (%)** 
   - **Average Tenure (Years)**

4. **Dashboard Development**
   - Built PivotTables from the Data Model; created PivotCharts and formatted them consistently.  
   - Added slicers for interactivity (e.g., Department, Designation, Gender, AgeGroup, SalaryBracket, TenureCategory).  
   - Layout: Title at the top left and KPI cards at the top right, slicers at left, below Title, main visuals arranged for quick interpretation.  
   - Exported/placed visuals on a Dashboard sheet and refined visual formatting for presentation.

---

## 📈 Dashboard Visuals
- **Attrition by Department** — Bar chart (horizontal)  
- **Attrition % by Gender** — Donut chart  
- **Attrition % by Age Group** — Pie chart  
- **Attrition by Salary Range** — Column chart  
- **Attrition Trend by City** — Line chart  
- **Attrition by Tenure** — Area chart  
- **KPI cards** for headcount, active employees followed by total employees, total attritions, attrition %, and average tenure (years)
- **Short Key Insights** at the bottom of the dashboard

---

## 🔑 Key Findings
- **Overall Attrition Rate:** 37.1% (high — ~2 out of 5 employees leave).  
- **Departments with highest attrition:** Sales and Accounts.  
- **Tenure:** Employees with **5+ years** show the largest number of exits, indicating potential long-term retention issues.  
- **Salary:** Highest absolute attrition counts occur in the **75K+** salary bracket, implying issues beyond compensation (e.g., satisfaction or growth).  
- **Age Group:** **46+** age group has the highest proportion of exits (~37%).  
- **Gender:** Attrition distribution is roughly even across Male, Female, and Other categories.  
- **Location:** Cities such as **Delhi** and **Mumbai** show relatively higher attrition counts.

---

## 📌 Insights & Recommendations
- **Target Sales & Accounts** with retention programs: better incentives, clearer career paths, workload review.  
- **Address career progression** for long-tenured employees (mentoring, promotions, role rotations) to reduce 5+ years attrition.  
- **Investigate non-pay factors** for high-salary attrition (workload, recognition, managerial issues, role fit).  
- **Engage 25-35 and 46+ age group** via fast-track learning, mentoring, and visible growth opportunities.  
- **City-level actions:** design localized HR interventions where attrition is higher (Delhi, Mumbai).  
- **Use dashboard filters** to monitor changes over time and evaluate the impact of retention initiatives.

---

## 🛠️ Tools Used  
- **Microsoft Excel** (Power Query, Power Pivot, PivotTables, PivotCharts, Slicers)

---

## 📑 Additional Notes
- For cleaner presentation, only the **Dashboard** and **Dataset** worksheets are visible in the Excel file.  
- All supporting **PivotTable worksheets** (used to build visuals and KPIs) have been **hidden**.  
- If you wish to review or modify them, simply **right-click on any sheet tab → Unhide → Select the sheets**.

---
## 📷 Dashboard Preview
![Dashboard](https://github.com/manishrajpurohit1108/Excel-Project/blob/main/HR%20Attrition%20Dashboard.png)
