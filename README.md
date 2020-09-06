![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Women_government_GDP

# Tableau project

## Content

- Project Description
- Questions & Hypotheses
- Datasets
- Datasets organisation
- Tableau organisation
- Workflow
- Results
- Problems
- Organisation
- Links


## Project Description

The goal of the project was to analyse a potential correlation between the percentage of women with seats in the National Parliaments of the World countries and the Gross Domestic Product (GDP). The whole goal was to find a potential connection with women empowerment and the development of the country, assuming beforehand that women emancipation could be a perk of highly development countries and not so much underdeveloped countries with other priorities in the agenda at times. The project started in a worldwide focus and was narrowed down to recent years and focused on countries which stand out in both metrics throughout the Tableau story, highlighting them through plotting. 


## Questions & Hypotheses

The main hypotheses to tackle was the existence of a correlation between percentage of women in the Parliamente and GDP worldwide. With these two indicators, a more general inference could bloom that women emancipation, equality and governmental representation could be connected to the level of development of the country, in this case evaluated by the GDP. It was also relevant to compare the two metrics individually in a worldwide context and analyse their discrepencies. The focus was to evaluate the most recent year 2019 and also to analyse the last 5 years, to check if an average of them could be taken into analysis - no major discrepancies supported the hypotheses that their average could be used. Then, to focus the analysis on the countries that stand out in both metrics for a correlation, following a study case mindset.




## Datasets

In order to generate the Tableau visualisation, two datasets from https://www.worldbank.org/ were selected and merged. Both can be found in the folder "data" and are described in the following points:

1) CSV file "GDP"
- It contais the GDP in US$ yearly information of all countries 

2) XLS file "goverment"
- It contains the % of women in the national Parliaments throughout the years


## Datasets organisation

In order to merge and clean the datasets and get them ready for Tableau, Python and Pandas library were used. Both files were imported into python jupyter notebook, cleaned and merged after cleaning. I decided to analyse only the last 5 years since the temporal descripencies in the % of women in the government throughout the years can be very strong and the main goal was to check the correlation with GDP. Therefore, only the years 2015 to 2019 were selected to export into CSV to posteriori import into Tableau. The name of the CSV file is tableau_data. 



## Tableau organisation

The Tableau story "Women in Parliament and GDP" is organised as follows:

- Storypoint 1 "Distribution map 2019": Map with the distribuition of the metrics last year
- Storypoint 2 "Scatter plot 2019": Scatter plot to correlate both metrics last year
- Storypoint 3 "Year evolution GDP 2015-2019": Line plot to check in there are strong discrepancies over the last 5 years in countries' GDP
- Storypoint 4 "Year evolution women in parliament 2015-2019": Line plot to check in there are strong discrepancies over the last 5 years in percentage of women in national parliaments by country
- Storypoint 5 "Country analysis by metric chosen": dynamic bar plot, using averages of the last 5 years now supported by the former storypoints, where the countries and the metric to analyse can be chosen
- Storypoint 6 "Dashboard Top women and top GDP": Dashboard connected to another two worksheets, where the user can select the amount of countries to analyse and it gives the values sorted DESC. Created so that the user can manipulate the values wanted - although a top 3 study case comes in the end of the story
- Storypoint 7 "Box plot GDP 2015-2019": Box plot to confirm outliers, in this case to point out the richest countries. 
Box plot created 
- Storypoint 8 "Box plot women in parliament 2015-2019": Box plot to confirm outliers, in this case regarding women in parliament
- Storypoint 9 "Top 3 comparison": Analysis of the three countries with the highest values on each of the metrics, to have some relevant clustering/case study that makes the results more "readable" to stakeholders.

There are also 3 additional supporting worksheets to the story.


## Workflow

The workflow was very streamlined: first selectd data of a topic of interest. The topic desired would have to be in the social-environmental field. Second goal was to find CSV or XLS files that were fitting the topic goal. The goal was also to practice some data cleaning in Pandas, therefore to find at least two datasets with a topic that could be correlated. After finding them, the next step was to clean them, select the data of interest in Pandas and export the file. After that, the file was ready to use in Tableau. Already in Tableau, the starting point was a story set up and 12 new worksheets were created, 9 of them directly linked to the story, one just for reference and other two connected to the dashboard.  Before starting the story, I delineated the goals with each story point and started plotting according to them, as described beforehand. On Tableau, the goal was to try the different concepts learned in the lectures and labs.


## Results

The results didn´t prove the initial hypotheses: no correlation was found between GDP and percentage of women in the parliament. A deeper analysis would be needed, analysing other metrics as women population in the country, role of women in society, etc.



## Problems

The problems started with the dataset gathering. In the beginning, the goal was a much more complex database with four databases from different sources. Unfortunately, that would take a lot of time away from Tableau into data cleaning, which was not the goal of the project. Regarding Tableau itself, sometimes it was hard to recreate positive outcomes, too much trial and error. 


## Organisation

The repository is organised in:

1) Data_cleaning jupyter file with the cleaned data
2) CSV file tableau_data used into Tableau
3) READ.me file with the project explanation and links
4) data folder with the two datasets described beforehand

## Links

The links to repository is:

https://github.com/Brunadiasmiguel/Women_government_GDP

And Tableau:

https://public.tableau.com/profile/bruna8094#!/vizhome/Women_government_GDP/WomenintheParliamentandGDP

