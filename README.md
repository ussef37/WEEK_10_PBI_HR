# Power BI HR Analytics Dashboard

## Project Overview

This project focuses on building an advanced HR analytics dashboard using Power BI to help organizations monitor and analyze their workforce.

The dashboard enables leadership and HR teams to explore headcount, retention, turnover, and workforce demographics through interactive visualizations and KPI indicators.

The project demonstrates data modeling, advanced DAX calculations, and professional dashboard design, providing a complete analytical solution for HR decision-making.

---

## Business Context

Organizations need to track, understand, and anticipate workforce changes to optimize talent management.

The HR dataset contains information about:

* Employees and employment history
* Salaries and bonuses
* Departments and managerial hierarchies
* Demographic and educational data

The objective is to transform raw HR data into an interactive analytics platform that helps leadership make data-driven decisions.

---

## Project Objectives

* Design a Star Schema data model
* Build advanced DAX measures and HR KPIs
* Create a multi-page interactive Power BI dashboard
* Develop custom slicer panels and dynamic tooltips
* Apply professional dashboard UI/UX design principles
* Deliver a portfolio-ready analytics project

---

## Dataset Structure

### Employees

* Personal details
* Demographic attributes
* Education background

### Employment History

* Hire dates
* Termination data
* Job levels
* Department assignments

### Compensation

* Salary data
* Bonus information

### Organizational Structure

* Departments
* Managerial hierarchy

---

## Data Modeling

The project follows a **Star Schema architecture** to optimize performance and maintain a clean analytical model.

### Fact Table

**People Fact**

* Employee ID
* Hire Date
* Termination Date
* Salary
* Job attributes

### Dimension Tables

* **Department Dim** → Department, Sub-Department
* **Job Level Dim** → Job Level
* **Termination Dim** → Termination Type, Termination Reason
* **Demographic Dim** → Gender, Race, Age
* **Education Dim** → Education Level
* **Location Dim** → City, Country
* **Marital Dim** → Marital Status
* **Manager Dim** → Manager hierarchy (Level 1 → Level 4)

Relationships were configured with proper **cardinality and filter directions**.

---

## Data Preparation

Data cleaning and transformation were performed using **Power Query**.

Key preparation steps included:

* Importing People Data and Employment History CSV files
* Cleaning and transforming HR data fields
* Calculating employee age from date of birth
* Normalizing employee status (Active / Terminated)
* Converting salary values to currency format
* Cleaning manager hierarchy identifiers
* Disabling source table loading for model optimization
* Organizing source tables into a dedicated folder

---

## DAX Measures

A dedicated `_Measures` table was created to centralize all key calculations.

### Core KPIs

* **All Employees** – total number of employees in the dataset
* **Headcount** – number of active employees at a given point in time
* **Turnover Rate** – percentage of employees who left the organization during a period
* **Retention Rate** – percentage of employees retained during a period

Unused columns were hidden to maintain a clean semantic model.

---

## Dashboard Pages

### 1. Headcount Analysis

Key KPI:

* Total Headcount

Visualizations:

* Department distribution with drill-down
* Job level distribution
* On-site vs remote employees
* Headcount by city (map)
* Workforce demographics:

  * Gender
  * Race
  * Age groups
  * Education level
  * Marital status

Filters:

* Year
* Age
* Gender
* Race
* Education
* Location
* Job Level
* Department

---

### 2. Retention Analysis

Key KPI:

* Global retention rate

Visualizations:

* Retention by job level
* Retention by department
* Min-Max retention slope chart

Supporting metrics:

* Starting Headcount
* Ending Headcount

Dynamic field parameters allow users to change the analysis dimension.

---

### 3. Turnover Analysis

Key KPI:

* Overall turnover rate

Visualizations:

* Turnover trends over time
* Turnover by department
* Turnover by job level
* Turnover by location
* Termination type distribution
* Termination reason analysis

Detailed employee table includes:

* Full Name
* Termination Date
* Department
* Job Level

---

## Interactive Features

### Custom Slicer Panel

A collapsible slicer panel was implemented using bookmarks and buttons.

Features include:

* Hamburger menu trigger
* Semi-transparent background
* Centralized filter control
* Open/close bookmark states

Slicers include:

* Age
* Gender
* Race
* Department
* Sub-Department
* Education
* Job Level

The panel is replicated across all pages for a consistent filtering experience.

---

### Dynamic Tooltips

A hidden tooltip page provides detailed employee information when hovering over visuals.

Tooltip data includes:

* Full Name
* Hire Date
* Salary

Additional features:

* Top 20 salaries
* Bottom 20 salaries
* Conditional formatting:

  * High salaries → Green
  * Low salaries → Orange

---

## Landing Page & Navigation

The dashboard includes a dedicated landing page containing:

* Project title and description
* Navigation buttons
* Icons for visual navigation

Users can quickly navigate to:

* Headcount Analysis
* Retention Analysis
* Turnover Analysis

---

## Dashboard Design

The dashboard follows professional BI design principles:

* Harmonized color palette (primary orange theme)
* Clean layout structure
* KPI highlights
* Transparent slicer panels
* Bold white titles
* Hover effects on navigation buttons
* Professional typography

The design focuses on creating an **ergonomic, aesthetic, and presentation-ready dashboard**.

---

## Tools & Technologies

* Power BI
* Power Query
* DAX
* Data Modeling (Star Schema)

---

## Skills Demonstrated

* Data modeling
* HR analytics
* Advanced DAX calculations
* Interactive dashboard design
* Data visualization best practices
* Business intelligence storytelling

---

## Project Outcome

This project delivers a complete HR analytics dashboard capable of helping leadership teams:

* Monitor workforce size
* Identify turnover patterns
* Analyze retention trends
* Explore workforce demographics

The result is a professional BI solution ready for portfolio presentation or business use.

---

## Author

**Youssef Soufiane**
Data Analytics & Business Intelligence
