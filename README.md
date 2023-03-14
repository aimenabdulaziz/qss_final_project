# QSS Final Project 

Welcome to the repository for the final project of **Aimen Abdulaziz**, **Esmeralda Abreu**, **Bernardo Burnes**, and **Charlie Knight**. Our project aims to analyze the top reasons for enrollment before and after COVID-19, using data from the Social Impact Practicum's (SIP) START Information Reporting System (SIRS). Specifically, we will be examining data from 10 months before and 10 months after COVID-19 was considered a National Emergency on March 14, 2020. These data include encounters with law enforcement, emergency visits, physical restraint during crises, demographics, and intake information. Our research will focus on investigating the top reasons for enrollment pre and post-COVID-19, using a pre-post binary (March 14, 2020) to compare enrollment patterns. 

Thank you for visiting our repository, and we hope that our project will provide valuable insights into the impact of COVID-19 on enrollment patterns.

**NOTE**: This repository is a work in progress.

Project Milestones:
- [Milestone 1](https://www.overleaf.com/read/tycrnpqwcgtj): Narrowing Down and Reviewing Past Projects 
- Milestone 2: Cleaned the datasets and completed preliminary data analysis

## Notebooks

Project `.ipynb` Scripts:
- [00_data_cleaning_and_merging.ipynb](https://github.com/aimenabdulaziz/qss_final_project/blob/main/code/00_data_cleaning_and_merging.ipynb)
  - Input: SIP's START Information Reporting System (Dartmouth Data Set)
  - Functionality:
    - Cleans all presenting problems by making it lowercase
    - Eliminates "Other Presenting Problems" and checks the retention rate
    - Merges "demographic" and "presenting_problems_no_other" using Client ID
    - Drops observations that had other reasons
    - Subsets the data frame to an equal number of month pre and post covid start date
    - Cleans the data sheet based on living situation change

  - Output: 
    - Merged Clean Data for 
        - [clean_presented_problems.pkl](https://github.com/aimenabdulaziz/qss_final_project/blob/main/data/clean_presented_problems.pkl)
        - [demographics_aggression_problems.pkl](https://github.com/aimenabdulaziz/qss_final_project/blob/main/data/demographics_aggression_problems.pkl)
 
  
- [01_data_vizualization.ipynb](https://github.com/aimenabdulaziz/qss_final_project/blob/main/code/01_data_vizualization.ipynb)
  - Input: Clean data from 01_data_cleaning_and_merging.ipynb
  - Functionality:
    - Creates visualizations such as bar plots, line plots, and geovisualizations

  - Output: 
    - all the figures are linked [here](https://github.com/aimenabdulaziz/qss_final_project/tree/main/output/figures)

- [02_regression_model.ipynb](https://github.com/aimenabdulaziz/qss_final_project/blob/main/code/02_regression_model.ipynb)
  - Input: [clean_presented_problems.pkl](https://github.com/aimenabdulaziz/qss_final_project/blob/main/data/clean_presented_problems.pkl)
  
  - Functionality:
    - Perform Logistic Regression on disability level, gender, and state to see if there is any correlation between any of this dependent variables and prevalence of aggression.

  - Output: 
    - Regression outputs included in the notebook and research paper

## Repository Organization

This repository contains the following files:
```bash
.
├── LICENSE
├── README.md
├── code
│   ├── 00_data_cleaning_and_merging.ipynb
│   ├── 01_data_vizualization.ipynb
│   └── 02_regression_model.ipynb
├── data
│   ├── Borough Boundaries
│   │   ├── geo_export_5fbe1568-6d75-4853-9e07-5643fefb35c7.dbf
│   │   ├── geo_export_5fbe1568-6d75-4853-9e07-5643fefb35c7.prj
│   │   ├── geo_export_5fbe1568-6d75-4853-9e07-5643fefb35c7.shp
│   │   └── geo_export_5fbe1568-6d75-4853-9e07-5643fefb35c7.shx
│   ├── Dartmouth Data Set.xlsx
│   ├── NYS_Civil_Boundaries
│   │   ├── Cities_Towns.cpg
│   │   ├── Cities_Towns.dbf
│   │   ├── Cities_Towns.prj
│   │   ├── Cities_Towns.sbn
│   │   ├── Cities_Towns.sbx
│   │   ├── Cities_Towns.shp
│   │   ├── Cities_Towns.shp.xml
│   │   ├── Cities_Towns.shx
│   │   ├── Counties.cpg
│   │   ├── Counties.dbf
│   │   ├── Counties.prj
│   │   ├── Counties.sbn
│   │   ├── Counties.sbx
│   │   ├── Counties.shp
│   │   ├── Counties.shp.xml
│   │   ├── Counties.shx
│   │   ├── Counties_Shoreline.cpg
│   │   ├── Counties_Shoreline.dbf
│   │   ├── Counties_Shoreline.prj
│   │   ├── Counties_Shoreline.sbn
│   │   ├── Counties_Shoreline.sbx
│   │   ├── Counties_Shoreline.shp
│   │   ├── Counties_Shoreline.shp.xml
│   │   ├── Counties_Shoreline.shx
│   │   ├── Indian_Territories.cpg
│   │   ├── Indian_Territories.dbf
│   │   ├── Indian_Territories.prj
│   │   ├── Indian_Territories.sbn
│   │   ├── Indian_Territories.sbx
│   │   ├── Indian_Territories.shp
│   │   ├── Indian_Territories.shp.xml
│   │   ├── Indian_Territories.shx
│   │   ├── State.cpg
│   │   ├── State.dbf
│   │   ├── State.prj
│   │   ├── State.sbn
│   │   ├── State.sbx
│   │   ├── State.shp
│   │   ├── State.shp.xml
│   │   ├── State.shx
│   │   ├── State_Shoreline.cpg
│   │   ├── State_Shoreline.dbf
│   │   ├── State_Shoreline.prj
│   │   ├── State_Shoreline.sbn
│   │   ├── State_Shoreline.sbx
│   │   ├── State_Shoreline.shp
│   │   ├── State_Shoreline.shp.xml
│   │   ├── State_Shoreline.shx
│   │   ├── Villages.cpg
│   │   ├── Villages.dbf
│   │   ├── Villages.prj
│   │   ├── Villages.sbn
│   │   ├── Villages.sbx
│   │   ├── Villages.shp
│   │   ├── Villages.shp.xml
│   │   └── Villages.shx
│   ├── clean_presented_problems.pkl
│   ├── demographics_aggression_problems.pkl
│   └── ny_counties.pkl
└── output
    └── figures
        ├── aggression_by_gender_year.png
        ├── aggression_by_gender_ym.png
        ├── aggression_over_time_my.png
        ├── aggression_over_time_y.png
        ├── disability_by_state.png
        ├── disability_proportion_by_gender.png
        ├── disability_proportion_by_gender_2019_20.png
        ├── ny_agg_proportion.png
        ├── ny_agg_with_inset_map.png
        ├── ny_counties.png
        ├── presenting_problems_count.png
        └── presenting_problems_proportion.png
```