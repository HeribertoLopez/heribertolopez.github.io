---
title:  "Estimating the effects of income and race on homeownership rates in the United States from 2010-2019."
date:   2021-11-15
excerpt: "Undergraduate project for Statistical Modelling course at St. Olaf College " 
collection: portfolio
---  

# Introduction 

Homeownership rates serve as economic indicators of wealth for families across the United States. In the United States, owning a home is for many families a part of the American Dream
(Goodman, et al). However, the Pew Research Center reports that more U.S. households are renting now than at any point in the past fifty years (Ciluffo, et all). Homeownership rates are often not included in studies examining the economy, with income and unemployment as often
referenced factors. Recent economic hardships have placed a burden on American families and their ability to maintain a household. In order to positively affect the rate of homeownership we must understand what factors are associated with increased homeownership rates. A
study that investigated factors affecting household homeowenership in Hong Kong found that people view the high costs of living, housing sale prices and high deposits as factors
affecting homeownership decisons (Oladinrin, et al). Further research, using a cross-country analysis of homeownership data from the United Nations, showed that the sales price of
homes can have a negative effect on homeownership decisions. Moreover, increases in income are associated with increases in the percentage of consumers that choose to own households
for both developing and developed countries (Gwin, et al). However, the magnitude of income is found to be stronger for more developed nations.

We are interested in exploring how factors such as income and the percentage of race
demographics by regions of the United states have an impact on homownership rates. While previous literature has explored factors associated to homeownerhsip rates such as race and housing prices, there has not been substancial research on how factors such as income and race demographics are related to homeownerhsip rates and are different by regions of the
United States. Understanding how these factors are associated to homeownership rates by region will help inform policies aimed at increasing homeownership rates in the United States. 

# Material and Methods

The Federal Reserve Economic Data, otherwise known as FRED, and the United States Census Bureau were the two sources of our information. Specific to our research, FRED contained most of the data that was important. The annual data collected included unemployment
rate, homeownership rate, median family income, change in population, average home sales price, job openings, and new houses built for each region recognized in the US census. These regions were the Northeast, Midwest, South, and West. The data covered the years from
2000 to 2019. Job openings was missing data for the year 2000. This dataset included 80 observations of 9 variables. From the US Census Bureau, we collected the race demographics of each census region covering the years 2010 to 2019. This included total population of
each race and the percentage makeup. The data covered white, black, hispanic, asian, and other. This dataset included 40 observations of 7 variables. All of the data was exported and compiled in excel to create the datasets of information for each source. In order to create a single dataset for our research, the two datasets from FRED and theUS Census Bureau were joined together based on year and region. When combining the two datasets, only the percent race makeup of each region was used instead of total population of
each race. Within the new dataset, the data for population change, job openings, and housing starts were multiplied by 1000 as they were originally measured in thousands. Since the race demographic information was missing data for half of the years, we filtered the dataset to
cover the years of 2010 to 2019. This resulted in a dataset of 40 observations for 14 variables. Following this, we needed to mutate the scale of our variables to allow us to make conclusions from our results. The median income was put in terms of tens of thousands, sales price was
in terms of hundreds of thousands, and job openings was in terms of millions. The percent race demographic was multiplied by 100 to represent the percent as a whole number. After finalizing the data, we used the information to start looking at multilevel models
focusing on homeownership rate. Our exploration of different models began by performing exploratory data analysis and looking at the summary statistics for our variables. 

# Modelling 

To explore the factors associated with lower homeownership rates we modeled homeownership rates using a linear mixed model. Our linear mixed model included a multi-level linear model used to account for the similarity between regions as homeownership rates are likely to be
similar by region. In addition, an intercept for unemployment was included as a random effect for each region to account for unemployment similarities by region. Year, income, and the percentage of black population in a particular region were included as fixed effect predictors for homeownership. To choose our final model, we compared models based on
coeficient significance and likelihood ratio tests between models. Random effects were also estimated to determine whether there was variation between regions after accounting for year, income and the percentage of black.

# Results 

We found that the average homeownership rate in the data is 64.6%. However, the average homeownership by region has been decreasing since the year 2010 steadily (Figure 1) with slight increases in the years approaching 2019. Moreover, the higher the percentage of black
in the region the more the rate of homeownership decreased.(Figure 2). The relationship does not vary substantially by region. 

<center> 
  <figure class="half"> 
    <a href="/images/HomeOwnership_figure1.png"><img src ="/images/HomeOwnership_figure1.png"></a> 
    <a href="/imgages/HomeOwnership_figure2.png"><img src = "/images/HomeOwnership_figure2.png"></a>
    <figcaption> Figure 1. Homeownership rates and Income by region. (Left). Figure 2. Homeownership Rate and percentage black by region. (Right)<sub></sub></figcaption> 
  </figure>   
</center> 

# Discussion 

Based on our findings, we see that an increase in median family income or black population has a positive effect on homeownership rate in the United States, with median income having the greatest effect on homeownership of any of our variables. Our model also shows that each
increasing year is the main source of the declining homeownership in the US. In terms of race, this result goes against previous studies that show higher minority populations have lower homeownership than whiter areas. For income, this means that economic factors outside of
our model changing over the years is leading to the decline even though initial analysis showed a negative correlation between our variables. Although the median family income in the US is increasing, some other factor is resulting in the year over year decline of homeownership.
Some of these results may be explained by the randomization of unemployment.

The implications of this research is that other economic numbers should be explored to try and explain why homeownership rates are decreasing. There are some confounding variables that need to be accounted for. For median income, the racial demographics could affect those
numbers. Also, because our model used only the percent black population, the effect of each race was not explored which may be misleading. If other minority races were included, we may have found results that agree with previous research.

Given the scope of our research, the data analyzed can only be applied to the United States. Other countries may have different circumstances affecting the rate at which citizens own their homes. As previous studies have shown, the effect of income has a greater relationship
in developed countries. Also, this data can only be used on a broad scope in the US as the data was collected by region. It does not go in depth to reveal patterns within states or
communities.

This last point reveals a major weakness of our research. Data provided by the Federal Reserve only covered homeownership at the regional level. Each region contains a different number of states and each state would vary regarding economic and demographic factors.
This limitation of the four census regions restricted the breadth of our study and how many variables we could include. However, this still allowed us to make some key observations. A strength of our study was the multilevel aspect in which region and unemployment was
accounted for. This allows for our results to be used as a general overview for the United States and not overly influenced by one region’s numbers.

Further research needs to be performed with access to more specific numbers than the data available to us. Being able to analyze homeownership by state would allow for the implementation of more complex models that can account for multiple economic and demographic
factors. Whether it is not readily available or we were unable to find it, future studies using this information would be able to give more in depth analysis and find the factors that led to declining homeownership rates over the last couple decades. 


<center>
    <div class="btn-group", style="text-align: center;">
        <a href="https://github.com/HeribertoLopez/Home-Ownership-Project" class="btn btn-success"> Project Source Code</a>
    </div>
</center>

# References

Gwin, O. (2008). Do we really understand homeownership rates? An international study.
International Journal of Housing Markets and Analysis, 1(1), 52–67. https://doi.org/10.1108/
17538270810861157.

Goodman, L., & Mayer, C. (2018). Homeownership and the American Dream. The Journal
of Economic Perspectives, 32(1), 31-58. Retrieved November 3, 2020, from http://www.jstor.
org/stable/26297968 

Oladinrin, O. (2020). An analysis of factors affecting homeownership: a survey of Hong
Kong households. Journal of Housing and the Built Environment : HBE., 35(3), 939–956.
https://doi.org/10.1007/s10901-019-09723-
