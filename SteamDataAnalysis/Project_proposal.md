#PROJECT PROPOSAL:

The goal of this project is to predict the date and time and to suggest video games to a user, when a particular user logs in, based on the aspects like the type of video games he/she plays, age, location, steam rank etc. on the steam community website (https://steamcommunity.com/). Steam is a digital distribution platform developed by Valve Corporation, available on Windows, Os X and Linux. Basically, it is the PC gaming platform.This project can be deployed in the fields of marketing research, enabling the developers to develop a video gamewhich is best suited to a group of people. It can also be used to design a suggestion filter using which, a user can receive a list of suggested video games based on his/her user data.
#OVERVIEW: 
The sole purpose of the research is to analyze the steam data (age, location and game) of several steam accounts, and predict a Video Game for the user based on his/her age and location. However, this research could be even more accurate if we had considered a few more attributes like ‘Friend’s List’, ‘Number of Games’ etc. This research can also be deployed in a far greater scope, and can be used to suggest friends to a user based on the games played.

#DATASET: 
Collect data, which is as random as possible. Data Collection had to be done manually as Valve has denied Steam API key, which is required to access their data (We needed a premium account to receive API key). We have still managed to collect data from over 700 public steam accounts (out of 75 million). We considered only a limited number of games to save time. While collecting data, we noticed that many steam profiles had their ‘Age’ hidden, which left us with 2 choices: We either had to set it as a missing value, or move on to the next steam profile. Not many had their Location hidden, which easily made us set it missing value, rather than skipping the account. Given our limited time, it was highly unlikely for us to collect a lot of data, which might’ve actually greatly improved the accuracy. We planned on grabbing data from at least 20,000 steam accounts (out of 75 million), if we had the API key. Anything more than that much of data wouldn’t have been practical, given our limited processing speed. (Researchers from a website named Arstechnica had to scrape Steam for 80,000-90,000 steam accounts every day, for about 2 months just to find out the least played games on steam). Now, working on such a huge database, without limited resources, can prove to be really hard, at the moment. We finally were able to gather data from over 700 steam accounts, which resulted in about 1700 instances. Tried to be as diverse as possible, but we knew that, not all countries have equal number of players.

#CODE AND APPLICATION
Once we had the data, all that remained was to train and test the data using weka. We have used several algorithms to pick the best one to train the machine with. All these algorithms which we have used left us with an accuracy which averages around 50%. Before we can strike away the research saying that the accuracy is too low, we need to keep in our minds about the Redundancy. (I.e.; it is not necessary for a teenager from USA, to play a certain video game). We have decided to go by J48 algorithm to visualize the tree, and train our machine. For convenience and accuracy purposes.

#PROJECT MANAGEMENT
| TEAM MEMBER | ROLES AND SKILLS | CONTRIBUTION | 
|-------------|------------------|-------------------------------------------|
|Mounica Poreddy(999991539)|Data collection and API deleopment|Development of data sets and input data|
|Mohammed Shakeer Bandrevu(999991619)|Weka development|Usage of WEKA in process of development the project|
|Javeed Shaik|Coding|Development of prediction process|
|Yasmeen Kowsar Shaik(999991463)|Testing the reviews and code|
|SiriChandhana(999991460)|Reeporting|Final reporting|


#Check Points:
| CHECK POINTS | DATE	EXPECTED DELIVERABLE	| RESPONSIBLE TEAM MEMBER	| CHECKPOINT RESULT |
|---------------------|----------|-----------------|------------|
| 02/15/2016 |	Project Proposal |	Yasmeen Kowsar Shaik	| Submission of Group Project Proposal |
|03/08/2016	|Collection of datasets	|Mounica, SiriChandhana	|Collection of data from data source|
|03/20/2016	|Classification of datasets|	Mohammed Shakeer, Javeed 	|Classifying the reviews in to positive and negative.|
|04/15/2016	|Code development	|Javeed Shaik, Yasmeen Kowsar Shaik	|Developing the code for analysis|
|04/20/2016	|Testing|	Mohammed Shakeer Bandrevu	|Testing the code|
|04/30/2016	|Reporting|	SiriChandhana, Mounica	|Reporting the final project|
