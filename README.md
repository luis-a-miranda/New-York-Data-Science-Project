# New-York-Data-Science-Project

The goal of this project is to use data science methodologies to define and formulate a real-world business problem. 

The New York City Department of Housing Preservation and Development (HPD) needs to analyse data so that they can make data-driven decision making and decide how to approach their problems. The project is devided in 3 parts where:

1. Which type of complaint should the HPD focus on first?
2. Should the HPD focus on any particular set of boroughs, ZIP codes, or street (where the complaints are severe)?
3. Does the identified complaint types have an obvious relationship with any particular characteristic or characteristic of the houses?

## Results

1. The "Heat/Hot Water" is the one with the biggest amount of complaints. Therefore, the HPD should focus on fixing this complaint type first.

<img src="complaints_per_type.png" width="600">

2. Now, HPD can have 3 approaches and decide to fix problems by borough, zip code or street. The listed areas are the following:
 
<td><img src="complaint_per_borough.png" width=600></td>
<td><img src="complaint_per_15zip.png" width=600></td>
<td><img src="complaint_per_15streets.png" width=600></td>

3. Lastly, the mean values for any particular characteristic per complaint type is calculated and after a analysis of variance (ANOVA) is performed.

The F-test calculates the ratio of variation between groups mean, over the variation within each of the sample groups.
- Large F implies strong correlation, usually F>1 is a decent value.

 The p-value shows whether the obtained result is statistically significant.
- Small p implies strong confidence, usually p<0.05 is a decent value.






Copyright (c) IBM Corporation 2020.
