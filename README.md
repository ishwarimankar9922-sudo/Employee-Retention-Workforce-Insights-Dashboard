# HR Analytics & Employee Attrition Dashboard

## 📊 Project Overview

The **HR Analytics & Employee Attrition Dashboard** is an interactive Power BI project designed to analyze employee demographics, workforce composition, salary, job satisfaction, performance, and employee attrition.

The dashboard helps HR teams and business managers identify workforce trends and understand the key factors associated with employee attrition.

---

## 🎯 Project Objectives

* Analyze overall employee workforce data.
* Calculate and monitor employee attrition rate.
* Identify departments and job roles with higher attrition.
* Analyze employee demographics such as age and gender.
* Understand the relationship between salary and attrition.
* Analyze job satisfaction and work-life balance.
* Compare employee performance across departments.
* Provide interactive insights using Power BI.

---

## 🛠️ Tools & Technologies

* **Power BI Desktop**
* **Power Query**
* **DAX**
* **Microsoft Excel**
* Data Cleaning
* Data Transformation
* Data Visualization
* Data Analysis

---

## 📁 Dataset

The project uses an HR employee dataset containing **1,000 employee records** and the following fields:

| Column             | Description                           |
| ------------------ | ------------------------------------- |
| Employee ID        | Unique employee identifier            |
| Age                | Employee age                          |
| Gender             | Employee gender                       |
| Department         | Employee department                   |
| Job Role           | Employee job position                 |
| Education          | Education level                       |
| Monthly Income     | Monthly employee income               |
| Years at Company   | Employee experience in the company    |
| Job Satisfaction   | Job satisfaction rating               |
| Performance Rating | Employee performance rating           |
| Overtime           | Whether the employee works overtime   |
| Work-Life Balance  | Work-life balance rating              |
| Marital Status     | Employee marital status               |
| Attrition          | Whether the employee left the company |

---

## 📌 Key KPIs

The dashboard includes the following key performance indicators:

* **Total Employees**
* **Active Employees**
* **Employees Left**
* **Attrition Rate**
* **Average Age**
* **Average Salary**
* **Average Years at Company**

### Attrition Rate

```text
Attrition Rate = Employees Left / Total Employees × 100
```

---

## 📈 Dashboard Pages

### 1. Executive Overview

Provides a high-level view of the organization's workforce.

Key visuals include:

* Total Employees
* Active Employees
* Employees Left
* Attrition Rate
* Average Salary
* Average Age
* Employee distribution by department

### 2. Employee Analysis

Analyzes employee demographics and workforce composition.

Includes:

* Employees by Department
* Employees by Job Role
* Employees by Gender
* Employees by Age Group
* Employees by Education
* Employee distribution by marital status

### 3. Attrition Analysis

Focuses on employee turnover and possible factors affecting attrition.

Includes:

* Attrition by Department
* Attrition by Job Role
* Attrition by Gender
* Attrition by Age Group
* Attrition by Salary
* Attrition by Overtime
* Attrition by Job Satisfaction

### 4. Salary & Performance Analysis

Analyzes compensation and employee performance.

Includes:

* Average salary by department
* Average salary by job role
* Performance rating
* Job satisfaction
* Work-life balance
* Salary vs. years at company

---

## 🧮 DAX Measures

Some of the main DAX measures used in the project are:

### Total Employees

```DAX
Total Employees = COUNTROWS(Sheet1)
```

### Active Employees

```DAX
Active Employees =
CALCULATE(
    [Total Employees],
    Sheet1[Attrition] = "No"
)
```

### Employees Left

```DAX
Employees Left =
CALCULATE(
    [Total Employees],
    Sheet1[Attrition] = "Yes"
)
```

### Attrition Rate

```DAX
Attrition Rate =
DIVIDE(
    [Employees Left],
    [Total Employees],
    0
)
```

### Average Age

```DAX
Average Age =
AVERAGE(Sheet1[Age])
```

### Average Salary

```DAX
Average Salary =
AVERAGE(Sheet1[Monthly Income])
```

### Average Years at Company

```DAX
Average Years at Company =
AVERAGE(Sheet1[Years at Company])
```

---

## 🔄 Data Preparation

The data was prepared using **Power Query** before creating the dashboard.

Main data preparation activities:

1. Checked column data types.
2. Checked for missing values.
3. Checked for duplicate Employee IDs.
4. Verified categorical values.
5. Converted numerical columns to appropriate data types.
6. Prepared the dataset for Power BI analysis.

---

## 💡 Business Insights

The dashboard can help HR teams answer questions such as:

* Which department has the highest employee attrition?
* Which job roles have the highest turnover?
* Does overtime affect employee attrition?
* Does job satisfaction relate to employee attrition?
* Which age groups have higher attrition?
* How does salary vary across departments?
* Which departments have higher average employee performance?
* How does work-life balance relate to employee retention?

---

## 📊 Dashboard Features

* Interactive KPI cards
* Department and role analysis
* Attrition analysis
* Salary analysis
* Employee demographic analysis
* Interactive slicers
* DAX-based calculations
* Power Query data transformation

---

## 📷 Dashboard Preview

Add screenshots of your Power BI dashboard here after completing the project.

Example:

```markdown
![HR Analytics Dashboard](images/hr_dashboard.png)
```

---

## 🚀 Project Workflow

```text
Excel Dataset
      ↓
Power Query
      ↓
Data Cleaning & Transformation
      ↓
Data Modeling
      ↓
DAX Measures
      ↓
Power BI Visualizations
      ↓
Interactive HR Dashboard
      ↓
Business Insights
```

---

## 📂 Repository Structure

```text
HR-Analytics-PowerBI/
│
├── README.md
├── HR_Analytics_Employee_Dataset.xlsx
├── HR_Analytics_Dashboard.pbix
│
└── images/
    └── hr_dashboard.png
```

---

## 🎓 Skills Demonstrated

This project demonstrates practical knowledge of:

* Data Analysis
* Power BI
* Power Query
* DAX
* Data Cleaning
* Data Transformation
* KPI Development
* Data Visualization
* Business Intelligence
* HR Analytics
* Business Insights

---

## 👩‍💻 Author

**Ishwari Mankar**

MCA | Aspiring Data Analyst

**Skills:** Power BI | Excel | SQL | Python | Data Analysis
