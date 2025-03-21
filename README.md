# Traffic Accident Severity in the U.S. (2016-2023) - A Statistical Survey
This project uses the "US Accidents (2016 - 2023)" dataset from Kaggle to examine important parameters affecting the severity of road accidents in the US.  The study investigates a number of connections between the severity of accidents and variables such regional variations, road infrastructure, and weather. The objective is to offer practical insights that might enhance traffic safety regulations and accident avoidance tactics.

Research Question:
The research question we aim to address in this study is: "What are the key factors influencing the severity of traffic accidents in the United States, and how do these factors vary across different regions and time periods?"
Curiosity about the relevance of our research question led us to consider its importance. The research has the potential to contribute to the development of more effective accident prevention strategies. By pinpointing the key factors contributing to severe accidents, authorities can implement targeted measures to reduce their occurrence. Gaining insights into the relationship between various factors and accident severity is a step towards creating safer road environments for all.

DATASET DESCRIPTION
The "US Accidents (2016 - 2023)" dataset is a comprehensive collection of information on traffic accidents that occurred in the United States over the period from 2016 to 2023. Each unit in this dataset corresponds to a single traffic accident, and the dataset contains various attributes describing different aspects of each incident.
Key Variables:
ID: A unique identifier for each accident record.
Country: Indicates the country where the city, where the accident took place, is located.
Source: The source of the accident report (e.g., Bing, MapQuest).
Severity: A categorical variable indicating the severity of the accident (ranging from 1 for low severity to 4 for high severity).
Start and End Time: Timestamps indicating when the accident occurred and when it was cleared.
Distance: The distance covered by the accident.
Description: A narrative description of the accident.
Weather Conditions: Information about weather conditions at the time of the accident.
Road Conditions: Details about the state of the road surface.
Visibility: Visibility conditions during the accident.

Analysis Done:
1) Chi Squared test
Employed the Chi-square test to explore the relationship between road features (e.g., junctions, bumps, signals) and accident severity

2) Analysis of Accident Severity Across States Using Road Extent Affected by Accidents across Different States
Calculated the 95% confidence intervals for the mean distance affected by accidents for each state. This approach allows us to understand the range within which the true mean distance is likely to fall, with a 95% level of confidence

3) Analysis of differences in the proportion of severity level 2 in states with the national proportion
The analysis focused on severity proportions at level 2 in different states and compared them with the national severity proportion. Specifically examined accidents falling within the severity scale of 2, considering them to be the most common occurrences in terms of severity.

4) Leading cause of accidents in first 10 states sorted by accident count and analysis of road accidents based on weather conditions
Analyzing the impact of various independent variables on accident rates in each state, we investigated correlations with
factors such as distance (indicating accident severity), weather conditions (e.g., wind speed, visibility), and road conditions (e.g., bumps, junctions).

5) Impact of weather conditions on the severity of the accident
Methodology:
There are these continuous weather variables: Temperature, Wind_Chill, Pressure, Visibility, Wind_speed, Humidity and Precipitation. Explored the relationship between distance impacted by the accident in miles (continuous variable) and the weather variables. Used the pairs method to see if distance showed any relationship between the weather variables.

## HOW TO RUN THE PROJECT
You can use R Markdown to run the project
### Dataset
Due the large size of the dataset, it was not feasible to add it to the repository. It can be downloaded from Kaggle using this link:
https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents?resource=download

Ensure the dataset is saved in the same working directory as the analysis.rmd file. Make sure to update the name of the dataset csv file in the source code in case you rename it.

### Dependencies
The following R packages need to be installed:
```R
install.packages(c("dplyr", "mosaic", "ggplot2", "MASS", "ordinal", "knitr"))
```
### To Run
Open the analysis.rmd file in R Markdown.
Install the dependencies if needed.
Run the file by clicking on the run button in the IDE.

For further details -statistical tools used, methodology, analysis results, interpretation of results and conclusion,
please refer to the Accident_Analysis_report.pdf