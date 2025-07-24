<img align="right" width="100" height="50" src="https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png"> 

# London Business Crime analysis 
### Navigation
* [README](https://github.com/Kaori61/crime-data-analysis/blob/main/README.md)
* [Clean data](https://github.com/Kaori61/crime-data-analysis/blob/main/dataset/data_cleaned.csv)
* [Raw data](https://github.com/Kaori61/crime-data-analysis/blob/main/dataset/raw_data.csv)
* [Exploratory data analysis (EDA)](https://github.com/Kaori61/crime-data-analysis/blob/main/jupyter_notebooks/exploratory_data_analysis.ipynb)
* [Statistical analysis](https://github.com/Kaori61/crime-data-analysis/blob/main/jupyter_notebooks/statistical_analysis.ipynb)
* [Dashboard](https://public.tableau.com/views/LondonBusinessCrimeAnalysis/Dashboard1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

<img src='images/toppage.png' alt ='Crime analysis cover image' width='300'>

[![test](images/toppage.png)](images/toppage.png)



**London Business Crime Analysis** is is a personal capstone project focused on the ETL (Extract, Transform, Load) pipeline, exploratory data analysis and statistical analysis in Jupyter Notebook and visualisations in Tableau. 

The project examines business-related crimes (any criminal offence that is committed against a person or property which is associated by the connection of that person or property to a business.) across London boroughs, using publicly available police data. The goal of this analysis is to uncover trends in types crimes, identify crime rates in different boroughs and generate insights to inform better resource allocation, operational improvement and prediction of seaonal trend.



## Dataset Content
* London Business Crime dataset is publically available data that can be downloaded from here [London Datastore](https://data.london.gov.uk/dataset/mps-business-crime-dashboard-data/). The data contains the last 2 years of a range of crimes such as date, borough, type of crime and more.


## Business Requirements
* Monitor borough performance.
* Identify crime types that need attention.
* Improve case closure rate.
* Identify which day of the week experience the highest levels of crime.

## Hypothesis and how to validate?
### 1. Certain crime have higher positive outcome rate than others.

How to prove it? - Compare positive outcome rates. 

<img src="images/outcome_rate.png" alt="Positive outcome comparison" width="600"/> 

The positive outcome refers to crimes that was handled successfully such as offender was charged, fined, cautioned or held accountable.\
*The graph shows a significant difference between the highest positive outcome rate (Drug Offenses – 63.1%) and the lowest (Vehicle Offenses – 1.2%). This supports the hypothesis that positive outcome rates vary across different types of crime.*


### 2. Number of crimes are decreasing over time.

How to prove it? - Line chart of monthly crime case.\
<img src='images/crime2023.png' alt='Total crime case in 2023' width='500'>\
<img src='images/crime2024.png' alt ='Total crime case in 2024' width ='500'>\
*On the top right hand side in Total Crime KPI, those visualisations show the total number of crimes each year. The visualisation disproves that the number of crimes are decreasing over time*


### 3. Crime frequency is significantly higher on weekday and during winter months.

How to prove it? - Create visulisation to show the distribution of crimes on weekday and month.

<img src="images/monthlycrime.png" alt="Crime frequency by month" width="500"/> 
<img src="images/weeklycrime.png" alt="Crime frequency by week" width="400"/>

*The visualisation proves that more crimes takes place on weekday adn during the winter months*

### 4. The types of common crime differ across boroughs.
    
How to prove it? - Visualise types of crime by boroughs.

<img src="images/hypothesis4viz.png" alt="Common crime in Top10 Boroughs" width="1000"/>
    
  *The visualisation disproves the hypothesis. While there are minor variations between boroughs, Theft consistently emerges as the most common type of crime across all areas.* 



## Project Plan
### High-level steps taken for the analysis.
* Data collection
* Data cleaning & transformation
* Exploratory data analysis (EDA)
* Statistical analysis
* Dashboard creation
* Insight generation

### Data management 
How was the data managed throughout the collection, processing, analysis and interpretation steps?
* Original data was kept as `raw_data.csv` as a reference.
* Data processing and calculation was done in Python asn Tableau.
* During interpretation, key metrics were visualised using bar charts, heatmaps and KPI.

### Rationale for research methodologies
- Data cleaning & transformation: This is a key preparation before performing any analysis for data integrity and reliability.
- EDA: I performed EDA to understand the data structure and patterns better so that I could generate meaningful insights from the analysis.
- Statistical analysis: Create regression model to predic the future trend
- Dashboard creation: Visualisation is to show key metrics and findings to the stakeholder

## The rationale to map the business requirements to the Data Visualisations
* Monitor borough performance.\
<img src="images/heatmap.png" alt ="Heatmap for crimes that has high resolution rate" width="500"/>\
*Heatmap can show the demographic of crime rates all at once so I decided to use this graph. \
Darker orange colour represents crimes with high resolution rate for specific crime in different borough.* 

* Identify crime type that need attention.\
<img src ='images/most_common.png' alt ='Most common crime at all time'>\
*The most common crime doesn't change over time based the analysis I performed therefore, I decided to put the results as KPI*

* Improve case closure rate.\
<img src='images/worst5.png' alt ='Worst 5 resolution rate crimes' width="500"/>\
*This is the list of crimes with the bottom 5 worst closure rates that needs to improve.\
There are 12 different crime types but I wanted to audience focus on the least ones so I made a bar chart with the worst 5*

* Identify day of the week that experience the highest levels of crime.\
<img src='images/weekday.png' alt = 'Most common day for crime to take place' width ='500'>\
*This was interesting findings addition to original business requirements. This could be used to guide effective resource allocation, improve operational planning and target interventions.*

## Analysis techniques used
### Data analysis methods used
- Data cleaning and transformation: Data contains over 400k rows which was causing issue so I sampled data to 10% of original data. Replaced null values with appropriate value. Converted some of the data types into appropriate data types. Checked for errors and typo in the variables. Created new columns for analysis.  
- Exploratory data analaysis: Used to understand crime distributions by type, borough and time.
- Statistical analysis: Aggregate data, create statistical comparison to understand if the difference in positive outcome rate is statistically siginificant in different location.Created regression model to predict the crime trend.  

### Limitations
* Data contain mostly categorical data which was problematic with statistical analysis. I perfomed feature engineering on those data for them to be able to make statistical calculation with the help of generative AI. I also had problems manipulating some data in Tableau as it wasn't numerical data.
- I wanted to create a map of the London Borough that shows the different crime rates in Tableau. However, Tableau doesn't contain London borough spatial data as default. I tried to install it in Tableau but wasn't successful. Instead, I created heatmap to show the demographic of crime rates in different locaitons.

### Generative AI
- I used generative AI to plan a project, brainstorming ideas and aid for code generation and optimisation.

## Ethical considerations
* This project uses anonymised, publicly available data with no personally identifiable information. Ethical considerations regarding privacy and confidentiality have been fully observed.


## Dashboard Design
### Access to my dashboard from here: [Business Crime Trends in London](https://public.tableau.com/views/LondonBusinessCrimeAnalysis/Dashboard1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
### Overview of dahsboard
I wanted to use consistent colour scheme to make the informstion easy to digest. I used highlighter to emphasise the focus point on each graph.

<img src='images/dashboard.png' alt='Dashboard image' width='1000'>

### Filter 
When viewer select the year, the graphs and KPIs show the correspondent result. As a default, the dahsboard shows overall results between 2023 and 2024.

<img src='images/d2023.png' alt='Filter year' width='800'> 



Similary to the filter above, when the viewer select the borough, graphs and KPI change accordingly.


<img src='images/borough_filter.png' alt='Filter borough' width='800'>

 
### Information button
Business crime and posiitve outcome can be misleading so I created infomation button that describe what they mean for accesssibility. When audience hover over the info icon, it'll show the meaning of those terms.git 
<img src='images/info_business.png' alt='Business crime info' width ='800'>
<img src='images/info_positive.png' alt='Positive outcome info' width='600'>


## Unfixed Bugs
* As mentioned in the 'Limitations' section, the dataset primarily consists of categorical variables. I aimed to display the percentage of crime outcomes in each tooltip, but some tooltips did not show the correct values. I attempted to recreate the logic and sought help from generative AI tools; however, I was unable to find a reliable solution. I suspect the issue stems from the way I transformed and aggregated the categorical data before visualising it. Despite various attempts, I was unable to resolve the inconsistency in how percentages were calculated and displayed.\
<img src="images/heatmap.png" alt ='Heatmap' width = '500'>


## Development Roadmap
* I had issues activating my Python virtual environment (`.venv`) in Git Bash while using the default MINGW64 shell — VS Code wasn't detecting the environment, and key packages like `pandas` weren't working. After some changes to `.bashrc`, Git Bash began launching in the MSYS shell, which added confusion by showing duplicate prompts like (`.venv`) (`.venv`).
With help from ChatGPT, I diagnosed the issue, fixed my .bashrc configuration, selected the correct interpreter in VS Code, and installed missing packages like ipykernel.
* Plotly wasn't working properly on Jupyter Notebook. It kept showing me the error message "nbformat >=4.2.0 isn't installed" even though I had correct version installed. Thanks to two of my fellow students Celia and Jane, who helped me fix this issue. I was able to create Plotly graphs. 
* I had issues with regression models. The first prediction model didn't include cyclical patterns so the prediction seemed incorrect. I used ChatGPT to create better prediction model to incorporate better feature and able to make prediction with improved R² value. 
* Raw dataset contians over 400k rows which caused error in pushing update in repository (I didn't realise the data contained over 400k of rows and didn't have problem pushing commits before changing the same size dataset). Initially created LFS to manage data size but it was also creating problems.So decided to sample data to make dataset more manageable. 


## Conclusion
* The total number of crimes increased by 3.7% from 2023 to 2024, while the positive outcome rate slightly declined by 0.4%. This may indicate a growing demand that is not being met by available enforcement resources.

* Westminster remains the borough with the highest crime volume in both years. Strengthening security measures in this area could help reduce overall crime figures.

* Theft continues to be the most common crime type, with little change year over year. Notably, theft also appears among the bottom 5 crime types for positive outcome rate, suggesting that this category warrants deeper investigation to identify patterns or trends that could improve resolution rates.

* Drug offences consistently show high positive outcome rates, indicating effective operations. Insights or operational strategies from this area could be adapted or shared to improve performance in lower-performing categories.

* Crime incidents are most concentrated on Wednesdays and Thursdays, suggesting that increased security presence during midweek may help prevent crimes and better protect business owners.

## Main Data Analysis Libraries
* Pandas - Used this to work with data sorting, filtering etc
* Numpy - Used this to do calculation with arrays
* Matplotlib - Created basic plots
* Seaborn - Created statistical visualisations like heatmap
* Plotly - Created interactive charts 
* Scipy - Created statistical analysis
* Scikit-learn - Used this to create regression model 
Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.


## Credits 

* [London crime dataset](https://data.london.gov.uk/dataset/mps-business-crime-dashboard-data/) - Dataset used for analysis.
* [GeekforGeeks](https://www.geeksforgeeks.org/) - Used to aid in code generation.
* [ChatGPT](https://chatgpt.com/) - Used to brainstorm ideas and optimise, generate and debugging code.
* [Microsoft Copilot](https://copilot.microsoft.com/chats/wf7sdTkkf6ywDqvFxCqJQ) - Used Copilit build in Visual Studio Code to optimise and debugging code.
* [11 Most Favorited Data Visualisations on Tableau Public](https://www.tableau.com/blog/most-favorited-data-visualizations-tableau-public?utm_medium=link&amp;utm_source=Tableau%20Public%20Promo%20Tile) - I got Tableau design inspiration from this article. 
* [Information mark](https://www.vecteezy.com/vector-art/32184554-info-help-sign-icon-vector-symbol-line-outline-art-black-and-white-information-bubble-speech-mark-isolated-pictogram-image) - Information mark in Tableau was taken from this page.




## Acknowledgements 
Everyone I mention here is very quick to respond to my query. I really appreciate their support when I needed it.
* Emma Lamont - Course facilitator at Code Institute. She gave me great support and advice whenever I needed.
* Celia Pires- aka Class Rep. Gave me great assist to fix my bug in the code. 
* Jane Weightman - aka the Brain. Very knowledgeable and supportive, helped me fix my bug, advice on image creation and inspirtion on navigation button.

