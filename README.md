CST 383 Weather Project

Team Members -
Arlon Arriola larriola@csumb.edu
Benjamin Mona bmona@csumb.edu 
Rahul Khurana rkhurana@csumb.edu 
Cristian Serrano crserrano@csumb.edu 

Introduction - 
When we first began this project we focused on brainstorming ideas and discussing what types of data we want to research. We eventually came to the conclusion that we wanted to study the weather and attempt to use this data to make predictions on the weather. We decided to attempt to create a system that can take in previous months of data on rainfall for any area, and predict future rainfall in that area. This project was chosen as we had decided that machine learning could be used to accurately predict various facets of the weather, such as future temperature or rainfall, and we thought that rainfall specifically would be a great starting point for a potential future in predicting weather patterns. 
The purpose of our research was to take in data from different sources and then train our model on this data. We specifically wanted to try and predict the precipitation for the month of April 2021. Our main focus for the project was to determine if, using machine learning, it would be possible to predict future rainfall given the data from previous months, and even previous years, for a given area. 

Selection of Data - 
For our dataset, initially we had attempted to use several other sources of data, including various API’s and sets of data, and they all worked to some degree. However, we ultimately decided against them, and decided to use the API with the most data available to us, which can be accessed here: https://visual-crossing-weather.p.rapidapi.com.
Using their API, we were able to access the data required for virtually anywhere in the world, with decades of data available.This data included things such as precipitation, humidity, cloud cover, temperature, visibility, and so much more. Of course, for the purposes of this project, we were mainly interested in the precipitation, although we did include every available column in our dataframe.
On this final project we did not use feature engineering, which is developing a feature from other features in order to create a more effective model. However, given our model and the use of kNN regression, we elected not to use these.. 

Methods -
No tools or materials were used or included to answer the research question. We only used the data that we were able to receive from this API.
API: https://visual-crossing-weather.p.rapidapi.com

Results - 
After training our model and selecting our predictors, we realized that actually we were able to answer our question. The answer is that we are failing quite badly at predicting the future with our historical data. Using the trainer from 2016-2020, we do considerably worse (around 6 times worse) than just blindly averaging the monthly rainfall from those prior years, when trying to predict the rainfall on any specific day in April. It is likely that attempting to model a system as complex as weather using simple historical data was fairly doomed, no matter what machine learning we used (kNN, linear, decision trees, etc) - as weather patterns can change based on drought patterns, storms, climate patterns such as El Nino/La Nina, or climate change.
Therefore the answer was that with our current model, no we are unable to predict precipitation using machine learning, given the limited data we used.
As far as visualizations go, we made a couple graphs. As with our homework we would be asked to create visualizations first, and then predictors and building a model. We held the same principle when it came to our project.  

Discussion -
The answer implies that our attempt at creating a model based on historical data will not be enough to predict precipitation. That there are most likely many key factors that we did not specifically implement, that are required to achieve a more accurate prediction.
Well according to science daily, scientists are only able to predict weather 9 to 10 days out. This is specifically for daily weather in the regions where most people live.
Therefore yes, our findings are inline with what researchers and scientists who try to predict weather have as an outcome. The reality is that it’s very difficult to predict weather, and that we can only do so with a short buffer of about 2 weeks. 
Source - https://www.sciencedaily.com/releases/2019/04/190415154722.htm
The perspective is that this particular research is not going to work using data science or machine learning. Clearly there are already people at work trying to predict the weather and they agree that the weather predictability horizon is about 2 weeks. Weather is unpredictable and there is a hard limit to how far in the future accurate predictions can be made. 
We believe that the API we used provided us with a ton of information and data, but it simply didn’t even come close to what we needed and how complex the models would have to be to make accurate predictions. Machine learning simply does not work for this research topic, given the scope we approached it with. It may have worked with more data, a more complex model, and more thought derived in weather prediction, but given how complicated the fields of meteorology and climatology are, it is likely that no available amount of data would be able to give us the results we desire.

Summary - 
So we started this project thinking that we would be able to use machine learning and historical data to predict weather, precipitation and patterns. We tried to focus our research particularly on anticipating the month of April and we did not do research on current weather prediction models. We actually did not know that scientists are only able to predict the weather up to a week or two. We found that after training our model, that we were nowhere close to predicting accurate weather and that a blind guess was on average 6 times more accurate. In conclusion, clearly the data we used and the predictors we selected were not enough to allow us to predict even a specific month. In fact it’s also important to realize that the models that are currently used to predict weather, encapsulate far greater amounts of data than the scope of our project. So our theory of being able to predict weather is already being used today consistently by researchers and scientists. However, there is a clear limit as to how far into the future weather forecasting can go and we were unable to even come close to predicting precipitation using our model. 
