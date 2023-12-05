# Data-Science-Job-Posting-Analysis

Examining the benefits, necessary qualifications, diverse locations, various companies, and additional insights derived from data extracted from California-based data science job postings in December 2021.

Dakota Doyle 

December 4, 2023 


## Introduction 
### The project was undertaken to explore and analyze California job postings specifically related to data science positions. The primary goal was to gain insights into the characteristics of these job postings, understand the demand for data science roles, and identify trends within the California job market. The research questions that guided this project were: 

1. What are the top 5 most common benefits amoung California Data Science Job Postings?
2. Is it required to have a Masters Degree, and is it benefitial based on salary?
3. What Cities and Companies are offering the Highest Salaries in California? 
4. What skills and qualiftaiations are most valuable?

### The project aimed to test the hypothesis that certain skills, qualifications, or industries dominate the data science job market in the state. The findings in this project are personal and helpful to me as I desire to become a Data Scientist after I graduate from Wentworth Institute of Technology in 2025. 

## Data 
### The datasets used in this project originated from Kaggle. They were comprises a comprehensive collection of job postings related to data science in California acquired on Decmber 17, 2021. The original raw data set of 1342 rows was cleaned and split into three subdata sets "benefits.csv" [preview data](/graphs/benefits_data_preview.PNG), "qualifications.csv" [preview data](/graphs/qualifications_data_preview.PNG), and "title_location_company_salary.csv" [preview data](/graphs/titlr_salary_company_location_data_preview.PNG) which are attached to this project folder. The datasets includes information on various attributes such as job title, company, location, required skills, qualifications, and industry. The title_location_company_salary.csv which contains the cleaned job titles, companies, locations, and salaries, qualifications.csv which contains the cleaned qualifications given by a binary matrix and is related to the title_location_company_salary.csv file by the index, and benefits.csv which contains the cleaned benefits given by a binary matrix and is related to the title_location_company_salary.csv file by the index. I further cleaned and analysised these sub-datasets individually as well as merged qualifications.csv and title_location_company_salary.csv back together in order to answer my third question.

## Methods 
![imported libaries](/graphs/imports.PNG)
### Through the course of this project, I initiated the refinement of the dataset by strategically eliminating irrelevant columns to narrow down the focus on the research question, thereby facilitating a more targeted analysis. Following this, I meticulously identified and removed empty and duplicate rows to uphold the integrity and accuracy of the data. Leveraging the power of the Pandas library, I employed a range of functions, including 'loc' to selectively choose columns of interest. Additionally, the integration of ['pd.merge'](/graphs/merging_QT_preview_and_code.PNG) and 'pd.csv reader' further enhanced the methodology, allowing for the efficient merging of datasets and streamlined reading of CSV files. I also implemented the Matplotlib and Seaborn libraries to utilize 'plt' for crafting visually informative plots and graphs. I specifically used pie charts as I found them to display the results best as most results are comparasion based. Finally, 'describe' and 'display/head()' were used for insightful statistical summaries and initial row exploration. These combined tools played a crucial role in contributing to a comprehensive and well-structured approach to addressing the research question.

## Results 
## Top 5 Common Benefits:
### The top 5 most common benefits among California Data Science job postings were identified: Health Insurance, Dental Insurance, 401(k), Paid Time Off, Vision Insurance. These benefits play a crucial role in understanding the comprehensive compensation packages offered in the field.

#### Result: Top 5 Most Common Benefits 

![top 5 benefits result](/graphs/top_5_benefits.PNG)

#### Bar Graph

![top 5 benefits bar graph](/graphs/top_5_benefits_graph.PNG)

#### Code

![top 5 benefits code](/graphs/top_5_benefits_code.PNG)



## Masters Degree Requirement and Salary Impact:
### Approximately half of the job postings indicated a preference or requirement for candidates with a Master's degree. The study suggests that having a Master's degree may be beneficial, as those with this qualification tend to have a higher maximum salary. However, it's noted that the mean salary increase is only slightly greater, implying a lower salary ceiling for those without a Master's degree.

#### I didvied the data into two groups, jobs with a Master's Degree required and jobs with no Master's Degree required. 
##### Here is the size of each group with 0.0 representing NO Master's Degree required and 1.0 representing Master's Degree required: 

![masters_degree_count](/graphs/masters_degree_count.PNG)

#### Here is a pie chart representing the precentage of jobs that do and do not require a Master's Degree, while it is close to 50/50 I would conclude from this that applicants with a Master's Degree do have the advantage as they qualifier for all postions while applicants without a Master's Degreee only qualify for less than half. 

![masters_required_pie_chart_graph](/graphs/masters_required_pie_chart_graph.PNG)


#### Data Statistical Description of Jobs with and without required Master's Degree 

![describe_no_masters_salary_result](/graphs/describe_no_masters_salary_result.PNG)

![describe_req_masters_salary_result](/graphs/describe_req_masters_salary_result.PNG)

#### We see that the mean salaries amoung the two subsets of the data only differ by an $10,000 increase in salary offered amound jobs that do require a Master's Degree, but I want to note the +$100,000 differnece in max salary for positions requiring a Master's Degree. 

![mean_salary_masters_vs_no_masters_result](/graphs/mean_salary_masters_vs_no_masters_result.PNG)


#### Code 

![masters_vs_no_masters_code](graphs/masters_vs_no_masters_code.PNG)

![counting_masters_degree_code](/graphs/counting_masters_degree_code.PNG)


## Cities and Companies Offering Highest Salaries:
### As shown in the pie charts below San Francisco emerged as a city with high-paying Data Science jobs, with Indeed being a prominent platform for such opportunities.

![top_20_highest_salaries_cities_pie_chart_graph](/graphs/top_20_highest_salaries_cities_pie_chart_graph.PNG)
![top_20_highest_salaries_companies_pie_chart_graph](/graphs/top_20_highest_salaries_companies_pie_chart_graph.PNG)
![top_20_highest_salaries_code](/graphs/top_20_highest_salaries_code.PNG)
![top_20_highest_salaries_results](/graphs/top_20_highest_salaries_results.PNG)


![extra_location_san_fran_extra_results](/graphs/location_san_fran_extra_results.PNG)
![extra_location_describe](/graphs/location_describe.PNG)
![extra_salaries_describe](/graphs/salaries_describe.PNG)
![extra_top_10_most_common_salaries_result](/graphs/top_10_most_common_salaries_result.PNG)

## Skills Desired in Postings:
### The study identified that a Master's degree, SQL, and C were among the most commonly desired qualifications. Interestingly, communication skills were emphasized more than analytical skills. 

![all_skills_code](/graphs/all_skills_code.PNG)
![all_skills_top_10_pie_chart_graph](/graphs/all_skills_top_10_pie_chart_graph.PNG)
![all_skills_top_10_results](/graphs/all_skills_top_10_results.PNG)

![common_coding_languages_code](/graphs/common_coding_languages_code.PNG)
![common_coding_languages_pie_chart_graph](/graphs/common_coding_languages_pie_chart_graph.PNG)
![common_coding_languages_results](/graphs/common_coding_languages_results.PNG)

![comparing_select_skills_code](/graphs/comparing_select_skills_code.PNG)
![comparing_select_skills_pie_chart_graph](/graphs/comparing_select_skills_pie_chart_graph.PNG)
![comparing_select_skills_results](/graphs/comparing_select_skills_results.PNG)


## Discussion 
### The implications of these findings and their significance are critical for both job seekers and employers in the field of Data Science. It is essential to consider how these results align with broader trends and insights from other researchers.

## Implications and Significance:
### The study's results have practical implications for job seekers, suggesting that pursuing a Master's degree may enhance earning potential. The emphasis on communication skills alongside technical expertise highlights the importance of well-rounded abilities in the field.

## Comparison with Existing Research:
### "Is a master’s degree in data science worth it?" by Meghan Malas emphasizes the surge in demand for data science professionals and the potential for lucrative salaries with a Master's degree. This perspective aligns with the current study's exploration, revealing a remarkable 480% increase in job opportunities for data science professionals since 2016. The significance of pursuing a master's degree in data science is underscored in both pieces, highlighting the potential for graduates to secure lucrative six-figure salaries.Insights from an Amazon business intelligence engineer, who secured a job offer before completing his master's, are featured in both articles, emphasizing the adaptability of a data science master's degree across diverse sectors. A deeper exploration of both studies could offer valuable insights into the evolving landscape of data science education and its impact on career outcomes. By comparing the findings, it becomes evident that the demand for data science professionals and the potential for substantial salaries with a Master's degree are consistent trends, providing a comprehensive perspective on the evolving requirements and opportunities in the dynamic field of data science.

## Perspectives for Future Research:
### Future research avenues could include a comparative analysis of the identified California trends with nationwide data. Additionally, delving into the accuracy of job postings, as suggested by the author, could uncover discrepancies between stated benefits and actual offerings.

## Exploration of Job Seeker Preferences:
### Investigating the alignment between job postings' requirements and what actual data scientists value in job offerings could provide a more nuanced understanding of the job market. This could include factors such as workplace culture, growth opportunities, and work-life balance.

### In conclusion, while the study sheds light on several aspects of California Data Science job postings, further research and exploration are warranted to deepen our understanding of the dynamics in this rapidly evolving field.

## References 

[Code](https://jupyter.cs.wit.edu/user/doyled3/notebooks/Data_Science_Fundamentals_Final_Project/data_science_job_posting_analysis_code_file.ipynb)

[Kaggle](https://www.kaggle.com/)

[Data](https://www.kaggle.com/datasets/michaelbryantds/california-salaries-in-data-science)

[Data Extracted From](https://www.simplyhired.com/search?q=%22data+science%22&l=California&job=XnAN-APSC0myGjJgTwz6gITa6jmIqgBTo-MAkT89bwMpGhVEokycrQ)

["Is a master’s degree in data science worth it?" By Meghan Malas](https://fortune.com/education/articles/is-a-masters-degree-in-data-science-worth-it/)

