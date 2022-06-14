# ETL DataWarehousing Project
## Introduction
The Tokyo 2020 Games were an unprecedented demonstration of unity and solidarity as the world came together for the first time following the onset of the COVID-19 pandemic for an Olympic Games focused on the pure essentials: a celebration of athletes and sport.


They showcase the evolution of the Olympic program, introducing new sports and events that strengthened the timeless appeal of the Olympic Games for a new generation. Tokyo Olympics had 339 events in 33 sports, this is the most sports in Olympic history


Data analysis will help us demonstrate with numbers how diverse and inclusive the Tokyo Olympics were.
## Project Goal
The goal of this project is to analyze the Tokyo 2020 Olympics dataset to discover meaningful information related to the athletes, disciplines, coaches, technical officials, and medals won during the Olympics.
* Business KPIs
```
Total medals won
Countries that received the most medals
Most popular sport and country with the highest number of participants
Gender of athletes across the top 10 disciplines
Country that has the most teams
Country that has the most coaches
Demographic of athletes and coaches 
Top 5 youngest athletes that competed 
Discipline that requires the most technical officials
```
* Technology to be used
```
ETL: Python, DBeaver
Database: AWS Redshift
Visualization: Tableau
```
## Dataset Link
This is an Olympic Games dataset that describes medals and athletes for Tokyo 2020. The data was created from the Tokyo Olympics.
More than 2,400 medals, and 11,000 athletes (with some personal data: date and place of birth, height, etc.) of the XXXII Olympic Games you can find here. Apart from it coaches and technical officials are present.

Data:
- medals_total.csv - dataset contains all medals grouped by country as here.
- medals.csv - dataset includes general information on all athletes who won a medal.
- athletes.csv - dataset includes some personal information of all athletes.
- coaches.csv - dataset includes some personal information of all coaches.
- technical_officials - dataset includes some personal information of all technical officials.

[Dataset URL](https://www.kaggle.com/piterfm/tokyo-2020-olympics?select=athletes.csv )
## Dimensional Model - Star Schema
Our dimensional model is created with 1 Fact table and 6 dimensional tables ( dim_technicals, dim_coach, dim_country, dim_athelet, dim_discipline and dim_medals). We decided to use the star schema, with the fact table surrounded by 6 dimensional tables since this schema is the most common and it is great for query, performance and analytics. 
![Model Image](C:/Users/nguye/Downloads/CIS 9440 - Data Warehousing/StarSchema.png)
