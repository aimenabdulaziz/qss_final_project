# QSS Final Project 

Welcome to the repository for the final project of Aimen Adbulaziz, Esmeralda Abreu, Bernardo Burnes, and Charlie Knight. Our project aims to analyze the top reasons for enrollment before and after COVID-19, using data from the Social Impact Practicum's (SIP) START Information Reporting System (SIRS). Specifically, we will be examining data from 10 months before and 10 monhts after COVID-19 was considered a National Emergency on March 14, 2020. These data include encounters with law enforcement, emergency visits, physical restraint during crises, demographics, and intake information. Our research will focus on investigating the top reasons for enrollment pre and post-COVID-19, using a pre-post binary (March 14, 2020) to compare enrollment patterns. 

Thank you for visiting our repository, and we hope that our project will provide valuable insights into the impact of COVID-19 on enrollment patterns.

Project Milestones:
Milestone 1: Narrowing Down and Reviewing Past Projects 
Milestone 2: Cleaned Data Frames and Graphs

- Project 01_notebook.ipynb Script

Input: SIP's START Information Reporting System (Dartmouth Data Set)

Functionality:
- Cleans all presenting problems by making it lowercase
- Eliminates "Other Presenting Problems" and checks the retention rate
- Merges "demographic" and "presenting_problems_no_other" using Client ID

Output: 
- Merged Clean Data for (demographics_problems_merged.pkl, emergency_crisis_services.pkl, in_patient_admissions.pkl, living_situation_change.pkl, presenting_problems.pkl)
- Figure "Frequency of Presented Problems"
- Figure "Living Conditions at Enrollment"
