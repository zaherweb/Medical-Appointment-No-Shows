

# Project: Investigate a Dataset (Medical Appointment No Shows)

## Table of Contents
<ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#wrangling">Data Wrangling</a></li>
<li><a href="#eda">Exploratory Data Analysis</a></li>
<li><a href="#conclusions">Conclusions</a></li>
</ul>




<a id='intro'></a>
## Introduction

A [US](https://www.scisolutions.com/uploads/news/Missed-Appts-Cost-HMT-Article-042617.pdf) study found that up to 30% of patients miss their appointments, and $150 billion is lost every year because of them.
Identifying potential no-shows can help healthcare institutions pursue targeted interventions  to reduce no-shows and financial loss.
This dataset collects information from 110,527 medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. 14 associated characteristics about the patient are included in each row.
The [Kaggle](https://www.kaggle.com/joniarroba/noshowappointments#) dataset comprised records from public healthcare institutions in a Brazilian city.

Data Dictionary:
01. PatientId:
Identification of a patient .
02. AppointmentID:
Identification of each appointment
03. Gender:
Male or Female . Female is the greater proportion, woman takes way more care of they health in comparison to man.
04. AppointmentDay:
The day of the actuall appointment, when they have to visit the doctor.
05. ScheduledDay:
The day someone called or registered the appointment, this is before appointment of course.
06. Age:
How old is the patient.
07. Neighbourhood:
Where the appointment takes place.
08. Scholarship:
True of False 
09. Hipertension:
True or False
10. Diabetes:
True or False.
11. Alcoholism:
True or False
12. Handcap:
0:4
13. SMS_received:
1 or more messages sent to the patient.
14. No-show:
True or False.


> ####  Question 1: (Who care most about his health and is there relation between health awareness  and attendance ...? )
> ####  Question 2: (Is  appoitment time affect and is their is relation between it and schedule time  ...? )








<a id='conclusions'></a>
## Conclusions

1.	we can see that people with age between 40 to 60 also between 0 to 10 care more than others regardless if they attended or not , but we focus now in most percentage in our data .
2.	we can see that females care more about their health regardless if they attended or not.
3.	For people who (**attended**)  with age between 40 to 60 also between 0 to 10 care more than other and that frequency of ages between 40 to 60 had been **increased** . 
4.	Percentage of (**female to male**) regardless to attendance  and after considering who attended increased from **2.012** to   **2.018** that mean female attended more than males .
5.	we can have conclusion that who care most with his health who has high probability to attend as we see in high frequency values for age between 40 to 60 and also as percentage of female to male .
6.	Ages in the range of 39 is highly probability to attend with percentage of 75.9 %.

7.	for people with no disability percentage of attendance is 71.426145049 % 

> A. for people with one disability percentage of attendance is 74.9367088608 % .
> B. for people with two disability percentage of attendance is 69.6428571429 % .
> C. for people with 3 disability percentage of attendance is 75.0 %
> D. for people with 4 disability percentage of attendance is 50.0 %

8.	Appointment day dosen't affect so much  for example this datas 16-5-2016 and 9-5-2016  has low percentage of attendance  both are monday so we can say that if the appointment is in monday the probability of patients to attend is low , but that's isn't totally correct as there are other mondays with high attendance . using line graph we can  see that there is no decision we can take upon day of appointment . we could think is another way of the period between schedule time and the appointment  
9.	person with waiting time of 30 day have high probability to not to come of 33%.
10.	After adding waiting time with age that helped to increase accuracy after combining both tech to 76.46% .










### Limitation 
1.	Our data isn’t similar to kaggle the data on kaggle is high version than what we work on For example handcap have 5 values (0 mean with no disability and 1 is with one disability and so on ) in previous version it had only  2 values true and false .

2.	AppointmentDay columns has the same time which is 00:00:00Z rather than ScheduledDay, but i don't think that would case problem.

3.	scheduled dates were after appointment dates and that’s not logically  true . 
4. Dataset was collected only in brazil  .
5. Dataset hav't a good description for it . 


5. So this applies only to the analyzed dataset. Statistical analysis was not carried out to verify whether the sample's representativeness in relation to the general population.


