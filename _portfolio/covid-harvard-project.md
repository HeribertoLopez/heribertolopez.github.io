---
title:  "Visualizing Covid-19 and Vaccinations"
excerpt: "Harvard summer program in biostatistics and computational biology project."
date: 2021-07-29
collection: portfolio
--- 

# Introduction 

COVID-19 is a type of coronavirus that possesses high rates of transmissibility among the human population.
For this research project, we investigated how COVID-19 cases change at varying degrees of vaccination rates from a global, country, and state-level perspective.
Our purpose was to identify the percentage of people vaccinated needed to begin to see a drop in cases.
A variant of the virus,  *Delta*, has recently been reported as having a higher rate of transmissibility among vaccinated and non-vaccinated individuals alike.
Previous research has shown that receiving two doses of the Pfizer mrna vaccine is highly effective across age groups greater than 16 years of age and in preventing symptomatic and asymptomatic SARS-CoV-2 infections. 
Moreover, the findings suggest that COVID-19 vaccination can help to control the pandemic. 
After gathering data for new covid cases, we analyzed how these cases respond to vaccination rates and drew conclusions from our findings.  

# Guiding Questions: 

- At what percentage of vaccinations do we begin to see a drop in cases? 
- How many weeks should we see a decline for the drop in cases to be attributed to vaccinations? 

# Data and Methods  

For this project, we used data from the our world in data database on github.  [Data on Covid-19 by *Our World in Data*](https://github.com/owid/covid-19-data/tree/master/public/data). As well as, data from the [*New York Times*](https://github.com/nytimes/covid-19-data). From the the *Our World in Data* dataset, we choose to use the following variables: location, population, date, new_cases, new_deaths, people_fully_vaccinated, and people_vaccinated. The dataset from the *New York Times* was used mainly to look at states in the United States. From the *New York Times* dataset, we choose the following variables:  date, cases, cases_avg_per_100k, deaths, deaths_avg_per_100k, people_fully_vaccinated, people_fully_vaccinated_per_hundred, people_vaccinated, people_vaccinated_per_hundred). Note that in both datasets, people_vaccinated refers to those that have received only one dose, and people_fully vaccinated refers to those that have received both doses or a single shot of a single dose vaccine. For our analysis of the data, we decided to create plots using shiny in R and estimate categorized cases and vaccinations by week, plotted change in weekly cases over amd weekly vaccinations over time and searched for trends and patterns within our plots. Additonally, we plotted new weekly cases vs. weekly vaccinations. 

# Conclusion and Findings 

From our plots, we saw that for countries with covid case reporting such as that of the US a drop in cases occurred when approximately five to fifteen percent of the population was partially vaccinated. We found that most countries have yet to control the pandemic. Moreover, there may be an increase risk posed from the presence of other variants. Below are a few of the graphs that we used to search for patterns, for more countries we included our source code and shiny app link for the project below. 

<center>
    <div class="btn-group">
        <a href="https://github.com/HeribertoLopez/Covid_19_Project/blob/main/Heri%20Folder/ShinyApp/app.R" class="btn btn-info"> Source Code</a>
         <a href="https://lopez-crypto.shinyapps.io/Final_Shiny/?_ga=2.9284149.1404967710.1626882075-1802921591.1626356006" class="btn btn-success"> Final Shiny App </a>
    </div> 
</center> 

<figure>
    <a href="/assets/img/covid-vax-cases-plot.png"><img src="/assets/img/covid-vax-cases-plot.png"></a>
    <figcaption> Rate of Covid Vaccinations in the United States over percentage of people fully vaccinated.</figcaption>
</figure>

<figure class="half"> 
	<img src="/assets/img/New Weekly Covid Cases.png">
	<img src="/assets/img/New_Weekly_Vaccinations.png">
	<figcaption> Plots Demonstrating New Weekly Cases and Vaccinations over time. Drops around January in the cases plot can be attributed to a drop in testing and reporting during the holidays. </figcaption>
</figure>

<br>

<figure>
    <a href="/assets/img/Cases vs Vaccinations.png"><img src="/assets/img/Cases vs Vaccinations.png"></a>
    <figcaption> New Weekly Covid Cases vs Percent of People Fully Vaccinated for a few selected countries.</figcaption>
</figure>
