# HR Employee Attrition Analysis Dashboard

## 📊 Project Overview

The **HR Employee Attrition Analysis Dashboard** is an interactive Power
BI dashboard designed to analyze employee workforce, attrition, salary,
job satisfaction, demographics, and other HR-related factors.

The dashboard helps identify patterns in employee attrition and provides
a clear overview of workforce and retention metrics.

> **Dataset:** Atlas Labs HR dataset (fictional/synthetic dataset)

## 🎯 Objectives

-   Analyze overall employee attrition.
-   Compare attrition across departments and job roles.
-   Understand the relationship between overtime and attrition.
-   Analyze employee demographics such as gender and age group.
-   Compare average salary across departments.
-   Study job satisfaction distribution.
-   Explore the relationship between employee age and salary.
-   Provide interactive filters for HR analysis.

## 🛠️ Tools & Technologies

-   **Power BI**
-   **Power Query**
-   **DAX**
-   **Data Visualization**
-   **CSV Dataset**

## 📌 Dashboard Features

### KPI Cards

-   Total Employees
-   Total Attrition
-   Active Employees
-   Attrition Rate
-   Average Salary

### Interactive Filters

-   Department
-   Gender
-   Job Role
-   OverTime
-   Business Travel

### Visualizations

-   Attrition by Department
-   Attrition by Job Role
-   Attrition by OverTime
-   Employees by Gender
-   Average Salary by Department
-   Age vs Salary
-   Job Satisfaction Distribution
-   Employees by Age Group

## 📈 Key Metrics

  Metric                 Value
  ------------------ ---------
  Total Employees        1,470
  Employees Left           237
  Active Employees       1,233
  Attrition Rate        16.12%
  Average Salary       112,956

## 🔍 Key Insights

-   The overall employee attrition rate is **16.12%**.
-   **237 employees** have left the organization.
-   The dashboard allows comparison of attrition across different
    departments and job roles.
-   Overtime status can be analyzed to understand its relationship with
    employee attrition.
-   Employee age groups provide insight into the composition of the
    workforce.
-   Salary differences across departments can be explored using the
    interactive dashboard.
-   Job satisfaction levels can be compared to understand employee
    experience.

## 🧮 DAX Measures

The project uses DAX measures such as:

``` dax
Total Employees = COUNTROWS(Employee)

Total Attrition =
CALCULATE(
    COUNTROWS(Employee),
    Employee[Attrition] = "Yes"
)

Active Employees =
[Total Employees] - [Total Attrition]

Attrition Rate =
DIVIDE(
    [Total Attrition],
    [Total Employees],
    0
)

Average Monthly Income =
AVERAGE(Employee[Salary])

Average Years at Company =
AVERAGE(Employee[YearsAtCompany])
```

## 📂 Dataset

The dashboard uses the **Atlas Labs HR dataset**, a fictional/synthetic
HR analytics dataset containing employee information such as:

-   Employee ID
-   Age
-   Gender
-   Department
-   Job Role
-   Salary
-   Business Travel
-   OverTime
-   Hire Date
-   Attrition
-   Years at Company
-   Job Satisfaction
-   Performance Rating

## 🖼️ Dashboard Preview

Add your Power BI dashboard screenshot to the repository and update the
filename below:

``` markdown
![HR Employee Attrition Analysis Dashboard](dashboard.png)
```

## 🚀 How to Use

1.  Download or clone this repository.
2.  Open the `.pbix` Power BI file using **Microsoft Power BI Desktop**.
3.  Review the dashboard and interact with the slicers.
4.  Select different departments, genders, job roles, overtime options,
    or business travel categories to explore the data.
5.  Use the visuals and KPI cards to analyze employee attrition.

## 📁 Suggested Repository Structure

``` text
HR-Employee-Attrition-Analysis-PowerBI/
│
├── HR_Employee_Attrition_Dashboard.pbix
├── dashboard.png
├── README.md
└── dataset/
    └── Employee.csv
```

## 👩‍💻 Author

**Dhavanithi**

MCA Student \| Data Analytics & Power BI Enthusiast

------------------------------------------------------------------------

⭐ If you find this project useful, consider giving the repository a
star!
