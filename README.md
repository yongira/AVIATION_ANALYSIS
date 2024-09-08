# AVIATION_BUSINESS_ANALYSIS
## OVERVIEW
This project requires use of data cleaning, imputation, analysis, and visualization to generate insights for a business stakeholder. 
## BUSINESS PROBLEM
The company is interested in purchasing and operating airplanes for commercial and private enterprises, but do not know anything about the potential risks of aircrafts. The project analyses which aircrafts are the lowest risk for the company to start the new business endeavor and the findings are translated into actionable insights that can be used to help decide which aircraft to purchase.
## DATA
The National Transportation and Safety Board has aviation accident data from 1962 to 2023 on civil aviation accidents and selected incidents in the United States and international waters. This is the data that will be analyzed to come up with concrete business recommendations.

We will be looking at data such as Aircarft Category, Make, Model, Injury Serverity, Aircraft Damage, Purpose of flight, Accident Causes, Phase of Flight, Weather Conditions, Aircraft age, frequency of accidents, etc.

This project deals with missing values, aggregating and visualizing data to help make data driven decisions for the organization.
## METHOD
### Dealing with Missing Data
We have to detect missing data first, then deal with them in order to move forward. We have three options for dealing with missing data --removing them from the dataset, keeping them, or replacing them with another value.
#### Remove
This is the easiest way to deal with missing values by dropping columns and/or rows. This is a valid strategy on very large datasets. 
For this strategy, it also does not matter if we are dealing with continous or categorical data.
#### Replace
We can also deal with missing values by replacing them with a common value. The downside of this is that it can introduce noise into our dataset.
#### Keep
Sometimes the knowledge that a value is missing can itself be informative for us. If knowing that a value is missing tells you something, then it is often worth keeping the missing values using the following strategies.

### Answering Identified Questions
We will answer the following questions with our dataset using Python.
    i). Filter aircraft makes and analyze there accident rates and severity.
    ii). Compare accidents by aircraft Make in relation to Broad phase of flight.
    iii). Assess which aircraft types handle poor weather conditions better, especially if your operations will involve flights in variable weather regions.
    
## RESULTS
Accident Distribution: the bargraph shows that CESSNA has the highest number of accidents (27,149), significantly more than any other make, followed by PIPER (14,870) and BEECH (5,372). BELL and BOEING have relatively lower accident counts, with BELL having the lowest.

![image](https://github.com/user-attachments/assets/35393033-9012-42c7-a096-03c8bdfa8092)

We get to assess which aircraft make handles poor weather conditions better, especially if operations will involve flights in variable weather regions. We focus on the total number of accidents under different weather conditions categorised as :IMC, VMC, and UNK/Unk. 

![image](https://github.com/user-attachments/assets/893b8669-62ce-43f0-a30f-28a2639e09d6)

Analysis of the aircraft make accidents with regards to the broad phase of flight. This analysis will help identify which phases of flight are most prone to accidents for each top 5 aircraft make.

![image](https://github.com/user-attachments/assets/7fa623bd-412f-4431-9206-d8cfbc0d0277)

## CONCLUSIONS
BELL's lower accident rate might suggest robust safety features or operational protocols. 
Least Affected by IMC: BELL has the lowest percentage of accidents under IMC (5.86%), suggesting it is the least affected by adverse weather conditions among the makes analyzed.
Overall Trends: While CESSNA has the highest total number of accidents, its proportion of IMC-related accidents is relatively low compared to its total, indicating a high volume of operations in VMC.
Significance: The lower IMC accident rate for BELL may reflect operational practices, aircraft design, or mission profiles that mitigate weather-related risks.

Landing and Takeoff: These phases are consistently among the highest for accidents across all makes, highlighting the critical nature of these operations.

Cruise Accidents: While generally considered a stable phase, cruise accidents are notably high for CESSNA and PIPER, possibly due to the high volume of flights or specific operational contexts.

Maneuvering: BELL shows a significant number of accidents during maneuvering, indicating a potential area for safety improvements.
## NEXT STEPS
More data could allow for further analyses and yield additional insights:
- Focus on filtering by different types of aircraft (e.g., small single-engine planes, multi-engine planes, commercial airliners, jets, helicopters). The objective would be to identify which aircraft types have the fewest accidents or the lowest accident severity (e.g., number of fatalities or injuries).
  
- Separate the data by commercial and private operations to compare risk profiles. This would compare the safety records of aircraft types used in private enterprises versus commercial operations. Commercial operations might have stricter regulations and maintenance practices.
  
- Include the aircraft age at the time of the accident, so as to determine if older aircraft models are more prone to accidents, which might influence decisions on purchasing newer aircraft.
    
## FOR MORE INFORMATION
See the full analysis in the **Jupyter Notebook** or review this **presentation**.
For additional info, contact Alison Peebles Madigan at yvonneongira@gmail.com
