#The effect of google search on actual unemployment
**Members of the group:**
* Bob Kruithof (864015/ U)
* Muriël Verbeek (422847/ U1244083)
* Manon Waals (402655/ U1257694)

##Research question
Can we predict the unemployment rate in the Netherlands with google searching? / Is there a correlation between google searching and the actual unemployment rate in the Netherlands?

##Motivation
This research is inspired by 'Detecting influenza epidemics using search engine query data' Ginsberg et Al. (2009). In this study they show they can estimate the level of influenza by looking at the online searching behavior of people. With online searching behavior we mean that when people feel sick they are looking on the internet for their symptoms. The conclusions they found are very important. With an early detection of the disease, in this case by looking at online search behavior, the impact of influenza can be reduced.  
In this research however we want to take a look at another important problem of the present days. We will investigate whehter we can predict the real unemployment rate in the Netherlands by using google searching. Information about the unemployment rate can be very important because online searching behavior of people, like in the case of influenza, can reduce the unemployment rate. This is the case because the government can take actions in an earlier stage before unemployment rate actually went up. In this research we will use google searching. We mean words such as 'niewe baan' ('new job') and uwv (which is an institution that helps unemployed people in the Netherlands to find a job).  

This study begins with a short summary about the method and the answer on the research question. Then we will give a more detailed explanation about the main assumptions and the data we used. This is followed by the results. We will end this study with a conclusion and discussion.

##Method
In this assignment we were able to find [data](https://github.com/ManonWaals/assignments/blob/master/Python.md#data) about both the unemployment rate in the Netherlands as well as data from google searching/google trends. For the unemployment rate we gathered data from Statistics Netherlands (CBS). For the google searching we decided to pick 6 words that we think are related with either unemployment or finding a new job. _blablabla.. wat we nog meer doen met data om tot antwoord te komen_

##Answer


##Main assumptions
* We assume that the words we pick from google trends are the most important words people search for.
* We assume that all words we pick are equally important and therefore get the same weight.
* We use the unemployment rate in the Netherlands which is adjusted for seasonal effects. We think that people who work only one season won't search for the words we pick.

##Importing packages and libraries
We used the following packages to run the model. 

**_Show packages and libraries_**

##Data
To answer the research question we used data of two different sources.

**Unemployment rate**  
First of all we used data about the unemployment rate. This data is gathered from [Statistics Netherlands (CBS)](http://statline.cbs.nl/Statweb/publication/?DM=SLNL&PA=80590ned&D1=10,12,14&D2=0&D3=0&D4=91-102,104-115,117-128,130-141,143-154,156-167,169-180&HDR=T&STB=G1,G2,G3&VW=T). We decided to look at the data from 2010 to 2015 and looked at the unemployment rate on a monthly basis. The unemployment rate we looked at is corrected for seasonal unemployment.

**_Show data from unemployment rate in tabel and show the graph_**

**Google Trends**  
The other source we used is [Google Trends](https://www.google.nl/trends/). We use index numbers for the amount of searches for specific words, that we think people will search for when they are unemployed. We have choosen 6 words, where some of them indicate search for unemployment benefits and others indicate searches for a new job. As for the unemployment rate we looked at the data from 2010 to 2015 in the Netherlands. We decided to use the following words: 'nieuwe baan' ('new job'), 'CV' ('resume'), 'vacatures' ('vacancies'), 'uwv' (an institution that helps unemployed people in the Netherlands to find a job), 'werkloosheid' ('unemployment') and 'werkloos' ('unemployed').

**_Show data from google trends in tabel and show simple graph_**

##Results


##Conlusion and Discussion

