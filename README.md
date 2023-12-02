# Data-Science-Job-Posting-Analysis
Analyzing benefits, required  qualifications, locations, companies, and more from data taken from California data science job postings in December 2021.


## readME DRAFT 
# Introduction	
Why was the project undertaken? What was the research question, the tested hypothesis or the purpose of the research?	10

    The project was undertaken to explore and analyze California job postings specifically related to data science positions. The primary goal was to gain insights into the characteristics of these job postings, understand the demand for data science roles, and identify trends within the California job market. The research questions guiding this project was: "1.What are the top 5 most common benefits amoung California Data Science Job Postings?, 2.Is it required to have a Masters Degree, is it benefitial based on salary?, 3.What Cities and Companies are offering the Highest Salaries in California and 4.What skills are most commonly desired amoung postings?  The project aimed to test the hypothesis that certain skills, qualifications, or industries dominate the data science job market in the state.

# Selection of Data	
What is the source of the dataset? Characteristics of data? Any munging, imputation, or feature engineering?	20

    The datasets used in this project originated from Kaggle. They were comprises a comprehensive collection of job postings related to data science in California acquired on Decmber 17, 2021. The original raw data set of 1342 rows was cleaned and split into three subdata sets "benefits.csv", "qualifications.csv", and "title_location_company_salary.csv" which are attached to this project folder. I further cleaned and analysised these sub-datasets individually as well as merged two back together in order to answer my third question. The datasets includes information on various attributes such as job title, company, location, required skills, qualifications, and industry.
    
"title_location_company_salary.csv which contains 1288 cleaned job titles, companies, locations, and salaries,

qualifications.csv which contains the cleaned qualifications given by a binary matrix and is related to the title_location_company_salary.csv file by the index, and

benefits.csv which contains the cleaned benefits given by a binary matrix and is related to the title_location_company_salary.csv file by the index."

* include rows size after my cleaning 

# Methods	
What materials/tools were used in answering the research question?	20

I used numpy, pandas, matplotlib.pyplot, and seaborn. 

I dropped columns I didn't deciser to use to make the data easier for me to focus on, I dropped empty rows and duplicate rows from the data. 

I used loc to select columns, plt to make plots and graphs, i used pandas, and i liked using describe and display/head() functions 

3 Results	
What answer was found to the research question; what did the study find? Any visualizations?	20

1. list top 5 
2. half jobs want it so i would reccomend it, also they do make more as the max is much greater but the mean is only slightly greater suggesting a lower max out 
3. san fran and indeed 
4. R and machine learing, and supprized that communcation skills was more than anaylsis skills 

# Discussion	
What might the answer imply and why does it matter? How does it fit in with what other researchers have found? What are the perspectives for future research?	20

I would love to research these reqults vs what actual data scienctist are looking for in job postings, I would also like to look at similar data USA wide and compare those results, and I would also like to question the accurance of the job postings because i would guess that the 50 postings not offering health insurance actually do offer it and just lack to mention it in the post. Also i wish python was a column amoung the dataset for qualifcations because i like it a lot better than R personally. 

*find other research make an article about masters degree 

# Coding	
ipynb file with clear comments and datafile.	10

# notes for me to edit readME later : 

# large text 
## medium text 
### small text 

## title 
- bullet indent 1
  - bullet indent 2 

` in this can not be changed, put code / makes shadow `

```
shadow
```

## reference 
[Reference1](link)
