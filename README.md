# Hospital-Emergency-Room-Dashboard-Excel-
Hospital Emergency Room Dashboard using Excel .

Hospital Emergency Room Dashboard – Monthly Report

This Hospital Emergency Room Dashboard provides a comprehensive monthly overview of patient flow, service efficiency, and demographic insights within a hospital’s emergency department. The dashboard is designed to help hospital administrators and healthcare analysts quickly monitor performance, identify bottlenecks, and support data-driven decision-making.
We need to create a Hospital Emergency Room Analysis Dashboard in Excel to improve efficiency and provide useful insights. This dashboard will help stakeholders monitor, analyze, and make better decisions for managing patients and improving services

Key Highlights

Total Patients: Displays the total number of patients visited during the selected month.

Average Wait Time: Shows the average waiting time (in minutes), helping assess operational efficiency.

Patient Satisfaction Score: Represents overall patient experience and service quality.


we are using Xalender Tble Formula and DAX Formulas :
Calendar Table Formula
         = List.Dates(#date(2023,01,01),731,#duration(1,0,0,0))

DAX Formula for Age Group : 
=IF([Patient Age]>=70,"70-79",IF([Patient Age]>=60,"60-69",IF([Patient Age]>=45,"45-59",IF([Patient Age]>=30,"30-44",IF([Patient Age]>=15,"15-29",IF([Patient Age]>=5,"05-14","0-4"))))))

DAX Formula For Patient Attend Status :
=IF([Patient Waittime]<30,"Within Time","Delay")

Visual Insights

Patient Attendance Status:
Pie chart comparing On-time vs Delayed patient attendance, enabling quick identification of service delays.

Gender-wise Analysis:
Donut chart showing the distribution of male and female patients visiting the emergency room.

Patients by Age Group:
Bar chart categorizing patients into age groups (0–9 to 70–79), helping understand which age segments require more attention.

Department Referral Analysis:
Horizontal bar chart showing the number of patients referred to different departments (General, Orthopedics, Cardiology, Neurology, etc.), highlighting departmental workload.


Interactivity & Filters
Month Selector: Allows users to view data month-wise.
Year Toggle (2023 / 2024): Enables year-to-year comparison for trend analysis.


Purpose & Use Case
This dashboard is ideal for:
Monitoring emergency room performance
Improving patient wait times and satisfaction
Understanding demographic patterns
Optimizing departmental resource allocation


Tools & Skills Demonstrated

Data Visualization & Dashboard Design
Healthcare Data Analysis
KPI Tracking & Reporting
Interactive Filters and User-friendly Layout
