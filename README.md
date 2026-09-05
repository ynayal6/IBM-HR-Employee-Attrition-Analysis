# 📊 IBM HR Employee Attrition Analysis

<img width="1241" height="647" alt="IBM HR Employee Attrition Analysis" src="https://github.com/user-attachments/assets/4214c072-8612-4f06-8a0c-897f208f352d" />

## 📌 Project Overview

Employee attrition is a major challenge for organizations because high turnover can increase recruitment costs, reduce productivity, and impact team performance.

In this project, I analyzed the **IBM HR Analytics Employee Attrition dataset** using SQL to identify the factors associated with employee turnover. The analysis focuses on department, salary, overtime, job satisfaction, work-life balance, age, and promotion history.

The project also combines multiple employee attributes to identify **employee profiles with particularly high attrition rates**.

---

## 🎯 Objectives

The main objectives of this analysis were to:

* Identify departments with the highest employee attrition.
* Understand the relationship between **salary and attrition**.
* Analyze the impact of **overtime** on employee turnover.
* Examine how **job satisfaction** relates to attrition.
* Evaluate the impact of **work-life balance**.
* Analyze attrition across different **age groups**.
* Investigate whether long periods without promotion are associated with higher attrition.
* Identify employee segments with the **highest likelihood of attrition**.

---

## 🗂️ Dataset

**Source:** IBM HR Analytics Employee Attrition Dataset

**Dataset:** IBM HR Analytics Employee Attrition & Performance

**Source:** Kaggle
`kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset`

---

## 🛠️ Tools & SQL Skills

* **SQL**
* CASE Statements
* Aggregations
* GROUP BY
* HAVING
* Subqueries
* Conditional Aggregations
* Data Segmentation
* Window Functions
* Business-oriented KPI Analysis
  
---

# 🔎 Analysis & Key Findings

## Q1. Attrition Rate by Department

This analysis calculates the employee attrition rate for each department by comparing the number of employees who left with the total number of employees in that department.

### Key Findings

<img width="417" height="87" alt="Screenshot 2026-09-05 at 10 43 03 AM" src="https://github.com/user-attachments/assets/3b375c4f-c892-43ca-a8eb-dfdc365150ed" />


### 💡 Insight

The **Sales department has the highest attrition rate at 20.63%**, making employee turnover a greater concern compared with HR and R&D.

Although R&D has the largest number of employees leaving in absolute terms, its larger workforce results in a lower overall attrition rate.

---

## Q2. Does Salary Affect Attrition?

Employees were divided into salary bands to examine the relationship between **monthly income and attrition**.

### Key Findings

<img width="293" height="111" alt="Screenshot 2026-09-05 at 10 45 12 AM" src="https://github.com/user-attachments/assets/cdd73080-758f-4092-89ef-eddd98de2083" />

### 💡 Insight

A clear negative relationship can be observed between salary and attrition.

Employees earning **below 3K have a 28.61% attrition rate**, compared with only **5.64% among employees earning 12K or more**.

This suggests that lower compensation is associated with higher employee turnover and highlights compensation as a potential area for retention strategies.

---

## Q3. Overtime and Attrition

This analysis compares attrition rates between employees who work overtime and those who do not.

### Key Findings
<img width="361" height="86" alt="Screenshot 2026-09-05 at 10 45 42 AM" src="https://github.com/user-attachments/assets/4a3dfcfc-b7f1-4440-b60f-b3063b5a80fb" />


### 💡 Insight

Employees who work overtime have an attrition rate of **30.53%**, nearly **3 times higher** than employees who do not work overtime (**10.44%**).

This makes overtime one of the strongest factors identified in this analysis and suggests that workload and working hours may be important considerations for employee retention.

---

## Q4. Job Satisfaction vs Attrition

Employee attrition was analyzed across four job satisfaction levels.

### Key Findings

<img width="456" height="124" alt="Screenshot 2026-09-05 at 10 46 21 AM" src="https://github.com/user-attachments/assets/e3bbf64c-3764-4e9f-b8f3-df8c748fdec3" />


### 💡 Insight

Employees with **low job satisfaction have the highest attrition rate at 22.84%**, while employees with very high satisfaction have the lowest rate at **11.33%**.

This indicates that employee satisfaction is associated with retention and highlights the importance of employee engagement and workplace experience.

---

## Q5. Work-Life Balance Impact

This analysis examines whether work-life balance is associated with employee attrition.

### Key Findings

<img width="343" height="109" alt="Screenshot 2026-09-05 at 10 47 02 AM" src="https://github.com/user-attachments/assets/5746d705-5404-4aeb-b239-b8957ccaa77c" />

### 💡 Insight

Employees reporting a **bad work-life balance have the highest attrition rate at 31.25%**, more than twice the rate of employees in the "Better" category at 14.22%.

The results suggest that poor work-life balance and workload management may be important factors associated with employee turnover.

Interestingly, the "Best" category has a slightly higher attrition rate than the "Better" category, showing that the relationship is not perfectly linear.

---

## Q6. Age Group Analysis

Employees were segmented into age groups to analyze attrition rates alongside average monthly salary.

### Key Findings

<img width="323" height="116" alt="Screenshot 2026-09-05 at 10 47 49 AM" src="https://github.com/user-attachments/assets/d3375e4a-3ada-4fba-b740-cf17d1181ba4" />


### 💡 Insight

The **Under 25 age group has the highest attrition rate at 39.18%**, followed by employees aged 25–35 at 19.30%.

Attrition decreases substantially among employees aged 35–45, reaching the lowest rate of **9.19%**.

The analysis also shows that average salary increases with age, while attrition generally decreases. This suggests that **career stage, compensation, and employee retention may be interconnected factors**.

---

## Q7. Years Since Promotion — Do Stuck Employees Leave?

This analysis investigates whether the time since an employee's last promotion is associated with higher attrition.

### Key Findings

<img width="311" height="123" alt="Screenshot 2026-09-05 at 10 48 31 AM" src="https://github.com/user-attachments/assets/eab98c2f-6c0a-4f49-bb5d-247523dd2784" />


### 💡 Insight

Employees who were **just promoted have the highest attrition rate at 18.93%**, while employees who have gone 3–5 years since their last promotion have the lowest rate at **10.13%**.

Employees with a promotion gap of more than five years also show relatively high attrition at **16.28%**.

This suggests that promotion history may be associated with attrition, although the relationship is not strictly linear.

---

## Q8. Profile of Employees Most Likely to Leave

This analysis combines **Department, Job Role, Overtime, Salary, and Promotion History** to identify employee segments with particularly high attrition rates.

Groups with fewer than 10 employees were excluded to reduce the impact of extremely small groups.

### Top High-Attrition Profiles

<img width="729" height="274" alt="Screenshot 2026-09-05 at 10 49 13 AM" src="https://github.com/user-attachments/assets/63bdad80-c012-4b3f-a6e6-5f1da6e37054" />


### 💡 Insight

The highest-attrition segment is **Sales Representatives who work overtime**, with an attrition rate of **66.67%**.

Overtime appears repeatedly among the highest-attrition employee groups, particularly in **Sales and Research & Development**.

Several high-attrition groups also have relatively lower average salaries, suggesting that **overtime, compensation, job role, and career progression may interact in influencing employee turnover**.

Even Sales Representatives who do not work overtime show relatively high attrition at **28.81%**, indicating that job role itself may also be an important factor.

---

# 📊 Overall Business Insights

Based on the analysis, several patterns stand out:

### 1. Overtime is strongly associated with attrition

Employees working overtime have a **30.53% attrition rate**, compared with 10.44% for employees who do not.

### 2. Lower salary groups have higher attrition

The lowest salary band has a **28.61% attrition rate**, compared with only 5.64% for employees earning 12K+.

### 3. Younger employees are more likely to leave

Employees under 25 have the highest age-based attrition rate at **39.18%**.

### 4. Poor work-life balance is associated with higher turnover

Employees reporting poor work-life balance have a **31.25% attrition rate**.

### 5. Job satisfaction is linked to retention

Attrition decreases from **22.84% among low-satisfaction employees** to **11.33% among very-high-satisfaction employees**.

### 6. Sales is the highest-risk department

Sales has the highest departmental attrition rate at **20.63%**.

### 7. Certain employee profiles are particularly high-risk

The combination of **Sales Representative + Overtime** produces the highest observed attrition rate at **66.67%** among groups meeting the minimum sample-size threshold.

---

# 🧠 Conclusion

This SQL analysis demonstrates how employee-level HR data can be transformed into actionable business insights.

The analysis indicates that **overtime, salary, age, work-life balance, job satisfaction, department, and job role** are all associated with differences in employee attrition.

The strongest patterns were observed around **overtime, younger employees, lower salary bands, and poor work-life balance**. Combining multiple dimensions also revealed specific employee segments with substantially higher attrition rates.

These findings can help HR teams prioritize areas for further investigation and develop more targeted employee retention strategies.

---
