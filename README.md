# QSS Final Project 

Welcome to the repository for the final project of **Aimen Abdulaziz**, **Esmeralda Abreu**, **Bernardo Burnes**, and **Charlie Knight**. Our project aims to analyze the top reasons for enrollment before and after COVID-19, using data from the Social Impact Practicum's (SIP) START Information Reporting System (SIRS). Specifically, we will be examining data from 10 months before and 10 months after COVID-19 was considered a National Emergency on March 14, 2020. These data include encounters with law enforcement, emergency visits, physical restraint during crises, demographics, and intake information. Our research will focus on investigating the top reasons for enrollment pre and post-COVID-19, using a pre-post binary (March 14, 2020) to compare enrollment patterns. 

Thank you for visiting our repository, and we hope that our project will provide valuable insights into the impact of COVID-19 on enrollment patterns.

**NOTE**: This repository is a work in progress.

Project Milestones:
- [Milestone 1](https://www.overleaf.com/read/tycrnpqwcgtj): Narrowing Down and Reviewing Past Projects 
- Milestone 2: Cleaned the datasets and completed preliminary data analysis

## Repository Organization

This repository contains the following files:
```bash
├── LICENSE
├── README.md
├── code
│   ├── 01_data_cleaning_and_merging.ipynb
│   ├── 02_data_analysis.ipynb
│   └── README.md
├── input
│   ├── Dartmouth Data Set.xlsx
│   └── README.md
└── output
    ├── README.md
    ├── demographics_problems_merged.pkl
    ├── emergency_crisis_services.pkl
    ├── figures
    │   ├── living_condition_at_enrollment.png
    │   ├── living_condition_at_enrollment_percentile.png
    │   └── presenting_problems_count.png
    ├── in_patient_admissions.pkl
    ├── living_situation_change.pkl
    └── presenting_problems.pkl
```

## Notebooks

Project `.ipynb` Scripts:
- 01_data_cleaning_and_merging.ipynb
  - Input: SIP's START Information Reporting System (Dartmouth Data Set)
  - Functionality:
    - Cleans all presenting problems by making it lowercase
    - Eliminates "Other Presenting Problems" and checks the retention rate
    - Merges "demographic" and "presenting_problems_no_other" using Client ID

  - Output: 
    - Figure "Frequency of Presented Problems"
    - Figure "Living Conditions at Enrollment"
  
- 02_data_analysis.ipynb
  - Input: SIP's START Information Reporting System (Dartmouth Data Set)
  - Functionality:
    - Cleans all presenting problems by making it lowercase
    - Eliminates "Other Presenting Problems" and checks the retention rate
    - Merges "demographic" and "presenting_problems_no_other" using Client ID

  - Output: 
    - A lot of tables and outputs inside the notebook
    - Figure [Frequency of Presented Problems](https://github.com/aimenabdulaziz/qss_final_project/blob/main/output/figures/living_condition_at_enrollment_percentile.png)
    - Figure [Living Conditions at Enrollment](https://github.com/aimenabdulaziz/qss_final_project/blob/main/output/figures/living_condition_at_enrollment_percentile.png)

