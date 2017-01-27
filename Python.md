#The effect of Google trends on actual unemployment
**Members of the group:**
* [Bob Kruithof](https://github.com/BobKruithof) (864015 / U1257965)
* [Muriël Verbeek](https://github.com/MurielVerbeek) (422847 / U1244083) 
* [Manon Waals](https://github.com/ManonWaals) (402655 / U1257694)

##Research question
Can we predict the unemployment rate in the Netherlands using data from Google trends?

##Motivation
This research is inspired by the paper ['Detecting influenza epidemics using search engine query data' by Ginsberg et Al. (2009)](http://www.nature.com/nature/journal/v457/n7232/abs/nature07634.html). In this study they show they can estimate the level of influenza by looking at the online searching behavior of people. Online searching behavior in this case is that when people feel sick, they look on the internet for their symptoms. By looking at online search behavior, influenza can be detected early and its impact can be reduced. 
In our research we want to take a look at another important problem of the present day and try to help solve it using searching behavior. We will investigate whehter we can predict the real unemployment rate in the Netherlands by using Google trends. We hope that the online searching behavior of people, like in the case of influenza, will help reduce the unemployment rate. Google trends data is available the moment it is being produced, while unemployment data often is announced with a certain lag. Thus, suppose that according to the Google trends data the unemployment rate has risen in this period, it might be usefull for policymakers to adapt a certain policy battling the unemployment. This policy can be adapted sooner than normal due to the use of Google trends. In our research we use Google trends to obtain data on the searching behavior of people. We look at the Google trends for words such as 'niewe baan' ('new job') and uwv (which is an institution that helps unemployed people in the Netherlands to find a job).  

This study begins with a short summary of the [method](https://github.com/ManonWaals/assignments/blob/master/Python.md#method) and the answer to the research question. Then we will give a more detailed explanation about the main assumptions and the data we used. This is followed by the results. We will end this study with a conclusion and discussion.
**_we need to link everything in the section above like method and answer and link it to our new file that includes the python codes. Also data below needs to be linked to the new file._**

##Method
In this assignment we were able to find [data](https://github.com/ManonWaals/assignments/blob/master/Python.md#data) about both the unemployment rate in the Netherlands as well as data from Google trends. For the unemployment rate we gathered data from Statistics Netherlands (CBS). For the Google trends we decided to pick 6 words that we think are related with either unemployment or finding a new job. After acquiring the data we calculated an average index of the 6 words we picked. All words got an equal weight. After plotting the average index we made a graph with both the unemployment rate and the index. To find whether we can predict the unemployment rate in the Netherlands using data from Google trends, we plot the data from both the unemployment rate and the Google trends to see whether the data has a comparable trend. Then we try to figure out whether we are able to not only compare the historic trends, but also see if we can use the historic data to predict the future. We do this by regressing the Google trends on the unemployment and using these coefficients to predict the future. **(??)**
**_add method for long term predictions_**

##Answer
We are indeed able to predict the unemployment rate in the Netherlands using data from Google trends when looking at the short term future.
**_add long term predictions answer_**

##Main assumptions
* We assume that the words we pick from Google trends are the most important words people search for.
* We assume that all words we pick are equally important and therefore get the same weight.
* We use the unemployment rate in the Netherlands which is adjusted for seasonal effects. We think that people who work only one season won't search for the words we pick.

##Importing packages and libraries
We used the following packages to run the model. 

**_Show packages and libraries_**

##Data
To answer the research question we used data of two different sources.

**Unemployment rate**  
First of all we used data about the unemployment rate. This data is gathered from [Statistics Netherlands (CBS)](http://statline.cbs.nl/Statweb/publication/?DM=SLNL&PA=80590ned&D1=10,12,14&D2=0&D3=0&D4=91-102,104-115,117-128,130-141,143-154,156-167,169-180&HDR=T&STB=G1,G2,G3&VW=T). We decided to look at the data from 2010 to 2015 and looked at the unemployment rate on a monthly basis. The unemployment rate we took is not corrected for seasonal unemployment as the Google trends data is also not corrected for seasonal fluctuations.

**_Show data from unemployment rate in tabel and show the graph_**

**Google Trends**  
The other source we used is [Google Trends](https://www.google.nl/trends/). We use index numbers for the amount of searches for specific words, that we think people will search for when they are unemployed. We have choosen 6 words, where some of them indicate search for unemployment benefits and others indicate searches for a new job. We decided to use the following words: 'nieuwe baan' ('new job'), 'CV' ('resume'), 'vacatures' ('vacancies'), 'uwv' (an institution that helps unemployed people in the Netherlands to find a job), 'uitkering' ('social security') and 'werkloos' ('unemployed'). For all words, we checked whether they could be associated with something different than unemployment. We found that this was only the case for 'CV' as people searching for this term also sometimes meant to search for boilers which are CV ketels in Dutch. To make sure that we only used the data of people that were searching for resume, we specified the 'CV' Google trend to the category 'vacancies and education'. As for the unemployment rate we looked at the data from 2010 to 2015 in the Netherlands.

**_Show data from Google trends in tabel and show simple graph_**

##Results


##Conlusion
As showed in the results, it is indeed possible to use Google trends to obtain information on the future unemployment rate earlier than when using the data on the unemployment rate from the CBS. So we are indeed able to predict the unemployment rate in the Netherlands using data from Google trends. However, this is a very short term prediction of only a couple of weeks. For longer run predictions.....
**_add long time predictions_**


##Discussion
Google trends fluctuate much and because of this our Google trends index has much more peaks and dips than the unemployment rate. We believe this is because unemployment rates are mcuh less easier to change than the amount of people looking at specific topics on Google, so the Google trends data is much more volatile than the unemploment rate. It would be beneficial to our research if we would be able to smooth the data that we obtained from Google trends in order to make it easier to compare it with the unemployment rates.
