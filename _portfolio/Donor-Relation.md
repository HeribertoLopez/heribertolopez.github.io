---
title:  "Constituent Behavior Associated with College Giving"
excerpt: "Exploring donor behavior and giving at St.Olaf College" 
date: 2021-05-02
collection: portfolio
--- 

# Introduction 

Many Colleges acrooss the U.S. are concerned about donors. However, while donor acquisition efforts are important, donor retention efforts have the ability to greatly increase
the amount of giving to an organization (Sargeant). The frequency of communication with constituents has shown the potential to affect a donors' decision to continue giving  to an organization (Deitz and Kellet).


For this project, we used data from a small liberal arts college and were interested in understanding the behavior of the donors for a particular college, specifically how
constituent' giving is affected by email communications. After an increase in email communications due to the COVID-19 pandemic, a leading question was how much email communication is too much? In our research, we used data from St. Olaf College Advancement's gift database and email database to examine donor engagement and behavior. We narrowed our data to focus just on alumni donations. The data used for the project was from St. Olaf's fiscal year 2020 (June 2019 - May 2020). 

# Data 

<figure>
    <a href="/images/Donor_Poster_1.png"><img src="/images/Donor_Poster_1.png"></a>
    <figcaption> </figcaption>
</figure>

Before begining, we filtered out all constituents who were not alumni of the college as the focus of our research was on the engagement of alumni. Afterwards, we noticed the donation amount distribution was heavily right-skewed (Figure 1.), so we filtered out gifts above the 99th percentile ($5000). Finally, we filtered out reocurring gifts (such as monthly $5 donations). The table below lists the definitions of the different segments analyzed. 


<figure>
    <a href="/images/Donor_Poster_1.png"><img src="/images/Donor_Poster_2.png"></a>
     <figcaption> Table 1. Description of the variables that were used. </figcaption>
</figure>

# Methods 

To explore our data we used the Kruskal-Wallis and the Wilcoxon-Mann-Whitney tests to determine whether there were significant differences in the median donation amounts among the different segments within the affiliation, leadership, and loyalty groupings. Additionally, we split the number of email messages received by constituents into brackets of 20 messages and used the Kruskal-Wallis test to determine whether there was a significant  difference in median donation amounts among the different message brackets. Because the donation amount was not normally distributed (Figure 1.), testing for a difference in medians was more appropriate than testing for a difference in means.

Logistic regression was also used to analyze the relationship between donors unsubscribing and the number of messages received, the number of messages clicked, the loyalty status of the donor, and the amount the individual donated to determine how St. Olaf Advancement should adapt their email communication strategy. The logistic regression in Figure 2 has been altered to show probability. The trend lines show the probability a constituent will unsubscribe from the mailing list based on the number of messages they have received.

# Results 

Using the Kruskal-Wallis test, we found a significant difference in the median giving amounts of the affiliation groups (H = 444.65, p-value < 0.001), the loyalty groups (H = 117.4, p-value < 0.001), and the message groups (H = 198.78, p-value < 0.001). Using the Wilcoxon-Mann-Whitney test, we found a significant difference in the median giving amounts of the two leadership groups (W = 421638, p < 0.001). 


<figure>
    <a href="/images/Donor_Poster_3.png"><img src="/images/Donor_Poster_3.png"></a>
     <figcaption> Figure 1. The skewed distribution of donoation amounts from Alumni. </figcaption>
</figure>




<figure>
    <a href="/images/Donor_Poster_4.png"><img src="/imges/Donor_Poster_4.png"></a>
     <figcaption> Figure 2. A line graph demonstrating the probability that a constituent within a given loyalty segment unsubscribes from the email list. 
     </figcaption>
</figure> 




<figure>
    <a href="/images/Donor_Poster_5.png"><img src="/images/Donor_Poster_5.png"></a>
     <figcaption> Figure 3. The average donation amount of constituents for each message bracket and leadership segment. 
     </figcaption> 
</figure> 

From our analysis of the visuals above, we noticed that the probability of unsubscribing based on the number of messages a constituent has received for each of loyalty groups does not fully demonstrate that as the number of messages increase the probability of unsubcribing will increase. Instead, it shows that if a given constituent is to unsubcribe, they will typically unsubcribe when the first few messages are received. Overall, the probability that a given constituent will unsubscribe is low if they’ve received a lot of messages and high if they’ve received only a few messages. It should be noted that some groups, such as the SYBUNT group, experience a slower decline in the probability of  unsubscribing.

# Discussion 

Based on the visualizations, we believe constituents are more sensitive to the first few messages sent compared to later messages. Moreover, we infer that constituents who prefer less emails will unsubscribe early on. From out data we found that the probability of unsubscribing is lowest for 1st Gift Last Year group and highest for the SYBUNT group. 

Our analysis of message brackets appear to show that donors in the lower message brackets appear to donate in larger amounts. Additionally, there is a larger drop in the average donation amount at the 80 to 100 message bracket. 

Based on these findings and limitations, believe that additional research should be done on other groups of constituents who may express different behaviors in response to email communications. It would be particular interesting to look at how far apart emails are sent to see if the timing of emails plays a role as well. Finally, exploration on the differences in behavior of the different messaging groups may be useful to further understand how to optimize messaging. 

# Sources 
- Sergeant, Adrian. Donor Retention: What Do We Know & What Can We Do About It?. Nonprofit Quarterly, 2013. 
- Dietz, R., and B. Keller. “Donor loyalty study: A deep dive into donor behaviors and attitudes.” Nonprofit Times, 2016. 
