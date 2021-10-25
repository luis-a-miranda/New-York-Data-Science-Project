# New-York-Data-Science-Project

The goal of this project is to use data science methodologies to define and formulate a real-world business problem. 

The New York City Department of Housing Preservation and Development (HPD) needs to analyse data so that they can make data-driven decision making and decide how to approach their problems. The project is devided in 3 parts where:

1. Which type of complaint should the HPD focus on first?
2. Should the HPD focus on any particular set of boroughs, ZIP codes, or street (where the complaints are severe)?
3. Does the identified complaint types have an obvious relationship with any particular characteristic or characteristic of the houses?

Dataset: [311 NYC Dataset](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0720EN-SkillsNetwork/labs/Module%201/data/311_Service_Requests_from_2010_to_Present_min.csv) obtained while enrolled on [Professional Certificate in IBM Data Science](https://www.edx.org/professional-certificate/ibm-data-science?index=product&queryID=f71f23095d28d770b5032557f7806f50&position=1).

## Results

1. The "Heat/Hot Water" is the one with the biggest amount of complaints. Therefore, the HPD should focus on fixing this complaint type first.

<img src="complaints_per_type.png" width="600">

2. Now, HPD can have 3 approaches and decide to fix problems by borough, zip code or street. The listed areas are the following:
 
<td><img src="complaint_per_borough.png" width=600></td>
<td><img src="complaint_per_15zip.png" width=600></td>
<td><img src="complaint_per_15streets.png" width=600></td>

3. Lastly, the mean values of house feature per complaint type is calculated and after an analysis of variance (ANOVA) is performed.

The top 5 and last 5 features are sorted by ascending F-test and can be seen in the following table:

| House Feature  | F-test     | p-value      |
| ---------------| ---------- | ------------ |
| NumFloors      | 351.770726 | 0.000000e+00 |
| BldgDepth      | 278.811181 | 0.000000e+00 |
| LotDepth       | 197.421067 | 0.000000e+00 |
| BldgArea       | 182.465668 | 0.000000e+00 |
| ResArea        | 172.946261 | 0.000000e+00 |
| ...            | ...        | ...          |
| OfficeArea     | 19.252312  | 1.215308e-52 |
| CommFAR        | 18.771666  | 3.792675e-51 |
| Lot            | 17.008696  | 1.105359e-45 |
| YearBuilt      | 13.150901  | 7.707729e-34 |
| NumBldgs       | 4.623433   | 5.831706e-09 |


Copyright (c) IBM Corporation 2020.
