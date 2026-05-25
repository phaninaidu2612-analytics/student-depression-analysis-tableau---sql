# Student Depression Analysis Dashboard | Tableau, SQL Server

## Tableau Public Dashboard link : 

### The project was done in trail version of tableau desktop , As the train ended hence could not be able to push it in tableau public as well. Will upload it soon.


## Dashboard Preview :

![1](https://github.com/user-attachments/assets/de0ac67f-d16d-43a1-a960-3af77ae0a261)

![2](https://github.com/user-attachments/assets/ebb0a701-6690-401c-871f-0360d6ff6c61)

![3](https://github.com/user-attachments/assets/7d772233-4b21-4649-86d3-a23d0544aa2b)

## Project Overview :

This project focuses on analyzing student mental health, academic pressure, lifestyle habits, and depression indicators using:

- SQL Server
- Tableau Desktop
- Tableau Public

The dashboard provides interactive visual insights into factors affecting student depression, including:

- Academic pressure
- Financial stress
- Sleep duration
- Study habits
- Suicidal thoughts
- Family mental health history

The project demonstrates:

- SQL Server data integration
- Tableau calculated fields
- Interactive dashboard navigation
- Modern UI/UX dashboard design
- Mental health analytics visualization

## Dataset Information :

The dataset contains student mental health and lifestyle-related attributes.

**Dataset Columns :**

| Column                               |
| ------------------------------------ |
| Gender                               |
| Age                                  |
| Academic Pressure                    |
| Study Satisfaction                   |
| Sleep Duration                       |
| Dietary Habits                       |
| Have you ever had suicidal thoughts? |
| Study Hours                          |
| Financial Stress                     |
| Family History of Mental Illness     |
| Depression                           |


## Data Source & Integration :
- Imported Excel dataset into SQL Server.
- Performed SQL-based data storage and management.
- Connected SQL Server database directly with Tableau Desktop.
- Published the final interactive dashboards to Tableau Public.

## Data Preparation & Transformation :

**Performed:**

- Data type validation
- Null handling
- Data consistency checks
- SQL-based preprocessing before Tableau integration

The cleaned dataset was then used for visualization and dashboard creation.

## Tableau Calculated Fields : 

**1. Depression Count:**

    SUM(
    IF [Depression] = "Yes" THEN 1 ELSE 0 END
    )

Used to calculate total students affected by depression.

**2. Suicidal Thoughts Count :**

    SUM(
    IF [Have you ever had suicidal thoughts] THEN 1 ELSE 0 END
    )

Used to calculate students experiencing suicidal thoughts.

**3. Depression Percentage :**

    SUM(
    IF [Depression] = "Yes" THEN 1 ELSE 0 END
    )
    / COUNT([Depression])

Calculates the percentage of students affected by depression.

**4.Suicidal Thoughts Percentage :**

    SUM(
    IF [Have you ever had suicidal thoughts] THEN 1 ELSE 0 END
    )
    / COUNT([Have you ever had suicidal thoughts])

Calculates the percentage of students with suicidal thoughts.

**5. Average Study Hours :**

    AVG([Study Hours])

**6. Average Academic Pressure :**

    AVG([Academic Pressure])

**7. Average Age Group :**

    AVG([Age])

## Dashboard Navigation & UI Features :

Implemented modern Tableau dashboard navigation techniques for an interactive user experience.

**Navigation Features :**

- Custom Tableau Navigation Buttons
- Transparent floating navigators
- Sidebar-based page navigation
- Interactive worksheet actions
- Clickable dashboard cards
- Cross-dashboard navigation


## Interactive Filter Navigation :

Implemented dynamic filters for:

- Gender
- Age Group
- Year Selection

using:

Use as Filter 
and Dashboard Filter Actions.


## UI/UX Enhancements : 
- Dark-themed professional dashboard design
- Neon-style icons and modern visuals
- Floating containers for responsive layout
- Transparent navigation overlays
- Interactive dashboard cards
- Consistent chart color palette
- Professional sidebar navigation experience

## Dashboards Included :

### Dashboard 1 – Student Mental Health Overview

Includes:

- Total Students KPI
- Average Study Hours
- Average Academic Pressure
- Depression Percentage
- Average Age Group
- Suicidal Thoughts Percentage

Provides a high-level overview of student mental health trends.

### Dashboard 2 – Student Depression Analysis : 

Contains detailed analytics and interactive visualizations for deeper exploration of mental health indicators.

#### Individual Analysis Pages / Worksheets

**Academic Pressure Analysis :**
 - Academic Pressure vs Student Count
    
**Financial Stress Analysis :**
- Financial Stress vs Student Count

**Study Satisfaction Analysis :**
- Study Satisfaction vs Student Count

**Sleep Duration Analysis :**
- Sleep Duration vs Student Count

**Study Hours Analysis :**
- Study Hours vs Student Count

**Age Group Analysis :**
- Mental health trends across age groups

**Gender Analysis :**
- Depression distribution by gender

## KPI Pages :

**Dedicated KPI pages for:**

- Total Students
- Average Study Hours
- Academic Pressure
- Depression Percentage
- Suicidal Thoughts Percentage
- Average Age Group


## Key Insights :

**Academic Pressure Impact :**

Students with higher academic pressure levels showed significantly higher depression indicators.

**Financial Stress Correlation :**

Financial stress emerged as a major contributing factor to student mental health concerns.

**Sleep & Mental Health :**

Students with lower sleep duration demonstrated higher depression percentages and reduced study satisfaction.

**Study Behavior Insights :**

Excessive study hours combined with low study satisfaction correlated strongly with mental health issues.

**Suicidal Thoughts Analysis :**

A notable percentage of students experiencing depression also reported suicidal thoughts, highlighting the importance of mental health awareness.

**Demographic Trends :**
Mental health patterns varied across:
- Gender
- Age groups
- Academic pressure levels

## Business / Institutional Impact :

This dashboard can help:

    Educational institutions
    Counselors
    Mental health professionals
    Student welfare departments

**to:**

- Monitor student well-being
- Identify high-risk groups
- Improve mental health initiatives
- Support data-driven intervention strategies

## Tools & Technologies Used :
- Tableau Desktop
- Tableau Public
- SQL Server
- SQL Queries
- Dashboard Navigation
- Tableau Calculated Fields
- Data Visualization
- Mental Health Analytics

## Conclusion :

This project demonstrates an end-to-end analytics workflow involving:

- SQL-based data integration
- Tableau dashboard development
- Interactive navigation implementation
- Advanced calculated fields
- Mental health trend visualization

The dashboard delivers actionable insights into student mental health, helping stakeholders better understand factors contributing to depression and emotional well-being.
