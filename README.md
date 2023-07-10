# data_science_project
Project 1 for data science

Worked on by Tarik Amraoui, Daniel Urbina and Ansel Obergfell


# Project Requirements

One of the main objectives of this course is to help you develop hands-on experience in analyzing complex data and building machine learning models. In this project, you will use a dataset from the open data portals to build at least two machine learning models to demonstrate your technical and analytical skills.

You can use the following tools to get the data for the project:

- NYC Open Data Portal - https://opendata.cityofnewyork.us/
- Open Data Discovery Tool - https://dd.akmislam.com/

In your project, you will complete the following tasks:

## **Task 1: Exploratory Data Analysis**

You will select a dataset from the open data portal that has a minimum of 10 features of which there will be at least one categorical and one numerical features. You will explain the insight of each feature: for example, their distribution,statistics etc and order the features based on their relationship with the target.

## **Task 2: Train Models**

You will train two models with at least three features and explain the optimization algorithms. If there are more than one optimization techniques available, try at least two of them and explain the difference.

## **Task 3: Test and Evaluate**

You will test both models using the test data and explain the evaluation metric with mathematical equations. If there are more than one evaluation metrics available, try at least two of them and explain the difference.

## **Task 4: Make Comparison**

Compare the test results of the both models and discuss the advantages and disadvantages of both models.

## Grading Rubric

- Does the presentation describe the data? ✔
- Does the presentation explain the main objective of the project? ✔
- Does the presentation explain the variations of similar models and specify which one best suits the main objective of the project? ✔
- Does the presentation clearly explain the key findings related to the main objective? ✔
- Does the presentation highlight possible flaws in the model and possible action to revisit the analysis with additional data or different modeling techniques? ✔
- Does the presentation follow a logical order? ✔
- Does the presentation define technical terms in a language appropriate for the target audience? ✔
- Is the length of presentation within the assigned time limit? ✔

# Project Analysis

## Task 1

1. **Selecting a dataset**: You are required to choose a dataset from an open data portal. An open data portal is a platform that provides access to publicly available datasets. You should browse through the portal and choose a dataset that interests you or is relevant to the topic of your assignment.
2. **Minimum of 10 features**: The dataset you select should have at least 10 different features. Features, also known as variables or attributes, are the columns or fields in a dataset that contain specific information. For example, if you were working with a dataset about cars, the features could include information such as the car's make, model, year, color, engine size, fuel efficiency, etc.
3. **Categorical and numerical features**: Among the 10 features, your dataset should include at least one categorical feature and one numerical feature. Categorical features represent qualitative data with distinct categories or groups, such as the car's make or color. Numerical features, on the other hand, represent quantitative data that can be measured or counted, such as the car's engine size or fuel efficiency.
4. **Explaining the insights of each feature**: Once you have selected a dataset and identified the features, you need to analyze and explain each feature. This involves examining the distribution, statistics, and other relevant information about each feature. For example, you could explore the distribution of car colors or calculate the average engine size across the dataset.
5. **Ordering features based on their relationship with the target**: The "target" refers to the variable or feature you are trying to predict or understand. In this case, you need to identify the target in your dataset (it might be explicitly mentioned or you may need to make a judgment based on the dataset's context). Afterward, you should analyze the relationship between each feature and the target. This could involve calculating correlations, performing statistical tests, or visualizing the relationships. Based on these analyses, you will order the features, indicating their strength or significance in relation to the target.

# Project Application

## Task 1: Exploratory Data Analysis

- Selecting a Dataset:
    1. Dataset Options (NYC Open Data):
        1. [~~Air Quality~~](https://data.cityofnewyork.us/Environment/Air-Quality/c3uy-2p5r)
        2. [~~2018 Central Park Squirrel Census - Squirrel Data~~](https://data.cityofnewyork.us/Environment/2018-Central-Park-Squirrel-Census-Squirrel-Data/vfnx-vebw)
        3. [~~Harbor Water Quality~~](https://data.cityofnewyork.us/Environment/Harbor-Water-Quality/5uug-f49n)
        4. [~~Youth Behavior Risk Survey (High School)~~](https://data.cityofnewyork.us/Health/Youth-Behavior-Risk-Survey-High-School-/3qty-g4aq)
        5. [~~New York City Leading Causes of Death~~](https://data.cityofnewyork.us/Health/New-York-City-Leading-Causes-of-Death/jb7j-dtam)
        6. [~~COVID-19 Daily Counts of Cases, Hospitalizations, and Deaths~~](https://data.cityofnewyork.us/Health/COVID-19-Daily-Counts-of-Cases-Hospitalizations-an/rc75-m7u3)
        7. [~~DOHMH New York City Restaurant Inspection Results~~](https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/43nn-pn8j)
        8. [**~~HIV/AIDS Diagnoses by Neighborhood, Sex, and Race/Ethnicity~~**](https://data.cityofnewyork.us/Health/HIV-AIDS-Diagnoses-by-Neighborhood-Sex-and-Race-Et/ykvb-493p)
        9. [~~NYPD Motor Vehicle Collisions Summary~~](https://data.cityofnewyork.us/NYC-BigApps/NYPD-Motor-Vehicle-Collisions-Summary/m666-sf2m)
        10. [**~~Motor Vehicle Collisions - Crashes~~**](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95)
        11. [**~~NYPD Arrest Data (Year to Date)~~**](https://data.cityofnewyork.us/Public-Safety/NYPD-Arrest-Data-Year-to-Date-/uip8-fykc)
        12. [~~NYPD Shooting Incident Data (Historic)~~](https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Historic-/833y-fsy8)
        13. [**~~NYPD Hate Crimes~~**](https://data.cityofnewyork.us/Public-Safety/NYPD-Hate-Crimes/bqiq-cu78)
        14. [E~~victions~~](https://data.cityofnewyork.us/City-Government/Evictions/6z8x-wfk4)
        15. [~~Parking Violations Issued - Fiscal Year 2023~~](https://data.cityofnewyork.us/City-Government/Parking-Violations-Issued-Fiscal-Year-2023/pvqr-7yc4)
        16. [**~~School Quality Report~~**](https://data.cityofnewyork.us/Education/2017-2018-School-Quality-Report-District-75-School/qy3b-p2ms)
    2. Dataset Options (Other):
        
        [2021-22-school-quality-guide-elementary-middle-school-data.csv](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8a89d946-cf66-413a-a811-e8bd1ab7a355/2021-22-school-quality-guide-elementary-middle-school-data.csv)
        
- Features (Feature (aka. column_name) - (Column Description)):
    1. ***enrollment*** - (Enrollment)
    2. ***survey_pp_RI*** - (Rigorous Instruction - Percent Positive)
    3. ************************************survey_pp_CT************************************ - (Collaborative Teachers - Percent Positive)
    4. ***survey_pp_SE*** - (Supportive Environment - Percent Positive)
    5. ***survey_pp_ES*** - (Effective School Leadership - Percent Positive)
    6. ***survey_pp_SF*** - (Strong Family-Community Ties - Percent Positive)
    7. ***survey_pp_TR*** - (Trust - Percent Positive)
    8. ***school_type*** - (School Type)
    9. ***Principal_experience*** - (Years of principal experience at this school)
    10. ***Teach_3_more_exp*** - (Percent of teachers with 3 or more years of experience)
- Categorical and Numerical Features:
    1. Categorical Features
        1. ***school_type*** - (School Type)
    2. Numerical Features
        1. ***enrollment*** - (Enrollment)
        2. ***survey_pp_RI*** - (Rigorous Instruction - Percent Positive)
        3. ************************************survey_pp_CT************************************ - (Collaborative Teachers - Percent Positive)
        4. ***survey_pp_SE*** - (Supportive Environment - Percent Positive)
        5. ***survey_pp_ES*** - (Effective School Leadership - Percent Positive)
        6. ***survey_pp_SF*** - (Strong Family-Community Ties - Percent Positive)
        7. ***survey_pp_TR*** - (Trust - Percent Positive)
        8. ***Teach_3_more_exp*** - (Percent of teachers with 3 or more years of experience)
        9. ***Principal_experience*** - (Years of principal experience at this school)
- Explaining the insights of each feature:
    1. Teacher 3 or more experience, and v enrollment
        
        
- Ordering features based on their relationship with the target:
    1. Target
        1. Years experience as principal
            1. Is a more experienced principal seen as a better leader?
            2. Does school size correlate with principal exp?
            3. Would larger schools experience higher burnout/turnover?
        2. Number of teachers with 3 years or more experience vs school size
    2. Features ordered based on the relationship with the target:
        1. insert here

## **Task 2: Train Models**

## **Task 3: Test and Evaluate**

## **Task 4: Make Comparison**
