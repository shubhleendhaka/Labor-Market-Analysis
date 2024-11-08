# Temporary Foreign Worker Program Labour Market Impact Assessment(LMIA) 2016-2023

This project aimed to develop a comprehensive view of the Labour Market Impact Assessments (LMIAs) issues for the Temporary Foreign Worker (TFW) positions in Canada for the year 2016-2023. 
An analysis of the data on positive and negative assessments by region, occupation, wage, and industry-specific programs (such as Seasonal Agriculture Worker Program) was performed along with assessing the program’s influence on the Canadian labor market across various industries and regions. The real life impact on the new measure of Employment and Social Development services was also suggested.

## Authors

- [@0x1AY](https://github.com/0x1AY)
- [@shubhleendhaka](https://github.com/shubhleendhaka)
- [@IskanderKenzhebekov](https://github.com/IskanderKenzhebekov)
- [@anahid-rr](https://github.com/anahid-rr)
- [@VioreliaM](https://github.com/VioreliaM)
- [@shriya-nit](https://github.com/shriya-nit)

## Data Collection and Transformation
- All Data was collected from the Open Canada Data Portal . Files included both positive and negative LMIA datasets spanning from 2016 to 2023
- Data Integration: Merged primary LMIA dataset with NOC and regional unemployment rate data to enhance analysis of employment trends and regional labor demand
- Pandas: For data manipulation and cleaning
- pgeocode: To convert postal codes to city names. enabling location-based analysis and enhancing the dataset’s geographical insights
- Standardization: Skipped title rows, trimmed irrelevant rows, and standardized column names across all files.

## Analysis and Key Insights

LMIA is a document that an employer in Canada may need to get before hiring a foreign worker. A positive Labour Market Impact Assessment(LMIA) indicates that there is a need for a foreign worker to fill the job and that no Canadian worker or permanent resident is available to do the job. In contrast, a negative LMIA indicates that the employer has not demonstrated a sufficient need for a foreign worker. 

The Canadian employment services divides the job category into different TEERs (Training, Education, Experience, and Responsibilities). The categories are:
- 0: Management responsibilities
- 1: Completion of a university degree
- 2: Completion of a post-secondary education program of two to three years at community college, institute of technology, or CÉGEP
- 3: Completion of a post-secondary education program of less than two years at community college, institute of technology or CÉGEP
- 4: Completion of secondary school
- 5: Short work demonstration and no formal educational requirements

1. LMIA applications by TEER:

   Below is a chart indicating that higher education (TEER 1 and TEER 2) lead to more positive LMIA outcomes.

<center>
   <video controls>
      <source src=”https://github.com/user-attachments/assets/06ef39f5-1ac2-4dd7-bf8c-206482c798f6.mp4” type=”video/mp4” />
   </video>
</center>

<div align="center">
  <img src="https://github.com/user-attachments/assets/06ef39f5-1ac2-4dd7-bf8c-206482c798f6" alt="Description" style="width:50%;">
</div>

2. LMIA applications by Provinces

   A video below of the dashboard shows that Quebec has the highest number of positive LMIA applications followed by Ontario and British Columbia while Ontario leads in negative LMIA applications. Although, the number of positive LMIA applications were not that high in New Brunswick, we can see higher density of positive LMIA in some areas in this Province.

<div align="center">
    https://github.com/user-attachments/assets/acfa67df-6e9f-4965-ac1a-5c260c70abe1.mp4
</div>

3. Changes to the low wage LMIA stream
   As of 8 Novemebr 2024, the employment and social development services announced new measures indicating that certain low-wage stream LMIA applications in work locations with an unemployment rate of 6% or higher at the time of LMIA submissionsubmitted as of September 26, 2024, won't be processed. Below you can see a map displaying the regions in Canada with positive LMIA in the low wage stream. Alberta has the highest number of low wage positive LMIA and it's unemployment rate in the month of September 2024 on an average is 8.45%. This indicates that Alberta could be one of the Provinces affected by this measure.

<div align="center">
  <img src="https://github.com/user-attachments/assets/5cc0531e-4ab7-48fb-a19d-7af21b2f16bf" alt="Description" style="width:80%;">
</div>

## Conclusions

- Positive LMIAs are most common in high-demand occupations such as computer programmers, general farm workers, and food service supervisors, reflecting ongoing labor shortages in these areas. In contrast, roles with more local availability, like general farm workers, often experience higher rates of negative LMIAs.

- Geographical analysis shows a correlation between regional unemployment rates and LMIA results, with regions experiencing higher unemployment often facing more negative LMIA outcomes. This emphasizes the role of local labor market conditions in determining LMIA outcomes.

- The analysis shows how policy makers can benefit from analyzing such datasets and use these insights to address labor gaps, plan workforce needs, or develop policy.

## Acknowledgements
- This project was done as part of Vancouver DataJam hackathon and I thank the organizers for conducting such an event
- Special thanks to Open Canada which was openly available for us to work on :https://open.canada.ca/data/en/dataset/90fed587-1364-4f33-a9ee-208181dc0b97/resource/b369ae20-0c7e-4d10-93ca-07c86c91e6fe and https://open.canada.ca/data/en/dataset/f82f66f2-a22b-4511-bccf-e1d74db39ae5/resource/94a0dbee-e9d9-4492-ab52-07f0f0fb255b
- Unemployment rates information: https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=1410035401&cubeTimeFrame.startMonth=09&cubeTimeFrame.startYear=2024&cubeTimeFrame.endMonth=09&cubeTimeFrame.endYear=2024&referencePeriods=20240901%2C20240901
