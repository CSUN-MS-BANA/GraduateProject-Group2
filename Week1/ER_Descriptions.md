Step 2: Develop an ER Model  

ER Model Description

|Entity |Relationship |Attributes|
Country            | 1-M |Country_ID, Country_Name|
Time               | 1-M |Year|
Country with Time  |Assc| Year_ID, Country_ID |
Population         | 1-1 | Population_ID, Country_ID, Total_Population, Urban_Pop, Pop_Growth, Age/Dependency_Ratio |
Economy            | 1-1 | Econ_ID, Country_ID, Year, GDP, GDP_Growth, GPD_Per_Capita, Exports, Imports, Domestic_Credit |
Health             | 1-1 | Health_ID, Country_ID, Fertility_Rate, Access_To_Elec, Air_Polution, Mortality_Rate
Education          | 1-1 | Education_ID, Year, Country_ID, Gender, Literacy_Rate,Education_Attain_Level,                     School_Enroll_Rate, Development_Score, Numeracy_Score, Socioemotional_Score
Employment         | 1-1 | Employment_ID, Year, Country_ID, Unemployment_%, Urban_Pop_%, Emp_by_Sector, Employmentcol, Gender_Specific_Empl, Age/Dependency_Ratio, Youth_Workforce_Ratio



The provided Entity-Relationship Model is designed to represent and organize a complex dataset comprising indicators related to Country Statistics, Economy, Health, Education, and Employment. The primary objective of this model is to see the relationship between different entities and help us in further analytics.
Entities:
Country: Serves as the central entity, uniquely identified by Country_ID. It connects all other entities, enabling regional analysis.
Attributes: Country_ID, Country_Name.
Time: Tracks the year of data collection or observation.
Attributes: Year.
Country with Time: Combines country and year to form an associative entity for time-series analysis.
Attributes: Country_ID, Year.
Population: Tracks demographic indicators.
Attributes: Population_ID, Total_Population, Urban_Pop, Pop_Growth, Age/Dependency_Ratio.
Economy: Captures economic metrics for each country and year.
Attributes: Econ_ID, GDP, GDP_Growth, GDP_per_Capita, Exports, Imports, Domestic_Credit.
Health: Represents health-related indicators for each country and year.
Attributes: Health_ID, Fertility_Rate, Access_to_Electricity, Air_Pollution, Mortality_Rate.
Education: Tracks education metrics, including gender-specific data.
Attributes: Education_ID, Gender, Literacy_Rate, Education_Attain_Level, School_Enroll_Rate, Development_Score, Numeracy_Score, Socioemotional_Scores.
Employment: Includes employment statistics categorized by gender, sectors, and unemployment rates.
Attributes: Employment_ID, Unemployment_%, Urban_Pop_%, Emp_by_Sector, Gender_Specific_Employment, Youth_Workforce_Ratio.


