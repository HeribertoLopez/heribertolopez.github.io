---
title:  "Estimating the effect of alcohol consumption on academic grades"
excerpt: "Undergraduate class project on the relationship between grades and alcohol." 
date: 2020-04-21
collection: portfolio
---


# Introduction

Colleges, Universities, and many schools across the world have implemented policies to tackle issues regarding alcohol use on their campuses. Many systems come with an effort to influence students to have control over their drinking habits and enjoy activities without feeling the need to feel inebriated. While schools seem to focus on the social aspects and harmful effects on individuals outside of academic life, researchers have developed a keen interest in the extent of the impact that alcohol has on the academic performance of students. The purpose of this study is to explore how alcohol consumption levels may influence the average final grade of students. 

Research on the effects of alcohol consumption is widely studied. Large areas of studies have focused on the social factors that may lead to binge drinking as students. A study published in 2014, "Just a First-Year Thing? The Relations between Drinking During Orientation Week and Subsequent Academic Year Drinking Across Class Years", gathered undergraduate participants from the University of Otago, New Zealand,  and collected survey data on the student participants for 13 days through daily diaries which included personal amounts of alcohol consumption. The study focused mainly on patterns for event-specific drinking, such as Orientation week. (Riordan, Benjamin, et. all). The results suggested that event-specific drinking is associated with increases in the amount of alcohol consumption across all class years. Similarly, other studies have looked at predictors surrounding alcohol and the association with poor academic achievement through survey and educational data of students (Walid et al.). But to what extent does alcohol influence academic performance?  

Of interest, when looking at the effects of alcohol, are potentially other factors that attributed to a change in academic performance. In the research article, "Legal access to alcohol and academic performance: Who is affected?" Austin and Joung use survey data to compare the average drinks students of legal age consume compared to those of younger generations. The results were similar to other studies where peers of legal drinking age showed a significant increase when obtained the legal drinking age compared to their younger peers.

Based on previous research, we expect that a model for alcohol consumption and final average grades of students will account for variables that have previously associated with the grades. Researchers Joung Yeoub and Austin Smith's model alone accounted for complexity variables such as individual effects on performance and normal variants that can significantly affect the academic grades of a student. Despite complex predictors associated with grades, we expect to uncover significant factors between alcohol consumption levels and the average final grades of students.  

# Methods

Our two datasets were obtained from Kaggle and included data collected thorough surveys from secondary school Portuguese students taking a mathematics course and a language course at two different schools the Gabriel Pereira (GP) and Mousinho da Silveira (MS) schools in Portugal. Our original dataset included a total of 662 students from which 395 students were taking a mathematics course, and 649 were taking a Portuguese language course, with 382 taking both classes. There were no missing variables present, and the average grades for each student were calculated over three academic year semesters. The grading system in Portugal secondary schools are graded differently than in the United States grades and are calculated between a 0 through 20 point scale (A = 20 - 18, B = 17 - 16, C = 15 -14, D = 13-12, E (Sufficient) = 11-10).  


<center>
    <figure class="half">
        <a href='/assets/img/Screenshot 2021-07-22 105348.png'><img src='/assets/img/Screenshot 2021-07-22 105348.png'></a>
         </figure>
</center>

For our exploratory analysis, we developed several plots and summary statistics for our predictors alongside our response to the average final grade of students. For our quantitative variables, we conducted histograms and for qualitative and binary variables used boxplots. Studies consisted of calculating means, medians, and standard deviations for each predictor and developing plots with the average final grade. A few predictors lead us to change our dataset. Most notably, we noticed that when looking at the relationship for the highest level of education for both mother and Father, we noticed that students who had parents with no education level had a slightly higher median than parents in the other groups. Students with parents in the no education level had a smaller sample size than those in the other groups, which is why their effect seemed to be more significant. We decided to remove them from our analysis and focus on parents with at least some education. 

After an analysis of each predictor with the response, we decided to explore relationships between variables. We investigated associations by creating similar plots to those we used with our response variable except now plotting them with each other. Further analysis that we did not included in the exploratory analysis was investigating differences in age by separating the quantitative variable into a variable called legal, where we split age by at the legal age of drinking to see if there were any differences. Similar approaches to other variables were done but were not entirely completed. 

Initial modelling was conducted using lasso and stepwise regression. Our process for modelling selection was based on the exploratory analyses with the intention to select the best model with the best possible combination of predictors for a student's average grade. Later on, we incorporated the cross validation method as well and decided to look at the affect of a model that is one standard deviation a way to adjust for model interpretability. Previous, analysis suggested that there was an interaction between alcohol consumption and sex

# Results

Our analysis suggests that weekend alcohol consumption is associated with the average final grade of students..However, the effect depends on the interaction between the weekend alcohol consumption and sex of the students. Furthermore, weekend alcohol consumption is not the only element that has an effect on the average grade of students. In our analysis, we have found that the mother’s education level also had an association with the average final grade of students. The mother’s education has a positive correlation with the average grade. On average, if the students are female, more weekend alcohol consumption is associated with higher average grades. However, for male students, more alcohol consumption is associated with lower
average grades.

The results of our study suggest implications on the increase in average grade for students who consume alcohol and are females. However, we also note that the average grade does not only have a correlation with students who consume alcohol but also has a correlation with the levels of a students’ mother’s education. Our model indicates that weekend alcohol consumption is not a terrible choice for all of the students. We could not ask every student to stop the weekend alcohol consumption in order for a better grade. For example, in our model, female students have higher average grades with more alcohol consumption on the weekend. These implications should be taken lightly as there were several limitations to this study. We can not neglect the limitation and problems in our research. First, we do not contain several predictors that have been associated in the past with effects on the average grade of students, such as workday alcohol consumption. Several other predictors that were also in our dataset did not make it in our final model due to lack of time and the complexity of the variables. In this case, we can not conclude that alcohol consumption has a positive or a negative effect on the average grade of students based on our dataset. Rather, there are some associations present. Another limitation is that our data was collected via a survey from students in secondary school. Our sample size was small for a high level of alcohol consumption. This may be a reasonable part of the reason why we do not have statistically significant for four predictors in Model2. Further research, should explore people who could extend the size of the population in the survey and contain workday alcohol consumption with a larger size of data. 

<center>
    <div class="btn-group">
        <a href="https://github.com/HeribertoLopez/Exploratory-School-Grades-And-Alcohol-Consumption-Project/blob/main/Final_Project.Rmd" class="btn btn-success"> Final Report  Draft Source Code (includes code for all plots made) </a>
    </div>
</center> 

# Sources: 

El Ansari, Walid., et al. “Is Alcohol Consumption Associated with Poor Academic Achievement in University Students?”. International Journal of Preventive Medicine, 2013.
Is Alcohol Consumption Associated with Poor Academic Achievement in University Students?  

Riordan, Benjamin C., et al. “Just a First-Year Thing? The Relations between Drinking During Orientation Week and Subsequent Academic Year Drinking Across Class Years.” Substance Use & Misuse, vol. 53, no. 9, 2018, pp. 1501–1510., doi:10.1080/10826084.2017.1415354. 
https://web-b-ebscohost-com.ezproxy.stolaf.edu/ehost/detail/detail?vid=0&sid=792a196f-9472-4864-b717-56cc6e6b832f%40pdc-v-sessmgr03&bdata=JnNpdGU9ZWhvc3QtbGl2ZQ%3d%3d#AN=130633250&db=aph  
