# 🏥 Hospital Healthcare Analytics Dashboard (Power BI)

## 📌 Project Overview
This project presents a **professional Power BI dashboard** designed specifically for **hospital and healthcare data analysis**.  
The goal is to transform raw medical and operational data into **clear, interactive, and actionable insights** that support hospital management and medical decision-makers.

The dashboard focuses on **patient flow, financial performance, medical services, and operational efficiency**.

---

## 🎯 Project Objectives
- Analyze hospital performance using **data-driven KPIs**
- Monitor **patient appointments, admissions, and services**
- Track **revenue from medical services, tests, and surgeries**
- Evaluate **doctors and departments performance**
- Support strategic healthcare decisions through visualization

---

## 🧠 Key Business Questions Answered
- How many patients are treated daily, monthly, and yearly?
- Which departments generate the highest revenue?
- What are the peak appointment times?
- Which medical services are most utilized?
- How efficient is resource and doctor utilization?

---

## 📊 Dashboard Features
### 🔹 Patient Analytics
- Total patients
- Appointments by date & time
- Patient distribution by department
- Surgery and test volume

### 🔹 Financial & Revenue Analysis
- Total hospital revenue
- Revenue breakdown:
  - Appointments
  - Medical tests
  - Surgeries
- Revenue trends over time

### 🔹 Doctors & Departments Performance
- Appointments per doctor
- Department-wise performance
- Doctor utilization rates

### 🔹 Interactive Filters
- Date range
- Department
- Doctor
- Medical service type

---

## 🛠 Tools & Technologies
- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Power Query (ETL)**
- **SQL / Excel (Data Sources)**
- **Healthcare KPIs & Metrics**

---

## 🧮 Sample DAX Measures
```DAX
Total Revenue =
SUMX ( Appointment, VALUE ( Appointment[fees] ) )
+ SUMX ( Patient_Tests, VALUE ( Patient_Tests[amount] ) )
+ SUMX ( Patients, VALUE ( Patients[surgery_charges] ) )
