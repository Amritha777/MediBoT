# MediBoT
# Team DRA Systems
## Summary :






## This was made as a part of the Hack4NSIT event

Due to information overload on the internet and the volume of result generated by search engines, it is difficult to get urgent solutions such as medical advice in a clean format. Also a symptom being suffered by an adult might be due to some other disease from that of a kid showing the same symptoms. Keeping these factors in mind we have ideated a solution that answers the mentioned problems and also bring on board a couple of more features to make it a wholesome healthcare assistant.

## Background:
With advances in machine learning, AI and allied fields computers have seen a revolution in the way they can use information. Our aim was to create a product that harness these power to provide crisp, clean and customised results.
The computers have become powerful enough to generate results on their own by looking at history and hence eliminating the need for hard coding each case. Plus they can improve their performance with time! So we can now analyse lots and lots of previous data to take present decisions based on them, this sounds a lot in sync with healthcare. The course of present medication is based majorly on past cases.
In fast response situations it matters a lot about what data is presented to  you and more importantly in what manner. It is very important about what you are being presented. For example in case of a wound a video showing how to dress it is far more effective than a write up but a write up is more apt for a flu.
With busy schedule missing once medication is a serious problem and it is quite a task to set reminders everyday for which medicine to take and till when.
Our goal was to develop a product which making the use of the above stated resources can provide a complete healthcare assistance at literally your beck and call. The aim was to make the bot as accurate as possible in  
1.	Diagnosing the specified symptom
2.	Succinct database 
3.	Notifying the user regarding her/his medication course.
We have developed the chatbot on Telegram, using BOT apis that use telegram messages as an interface. 

## Platforms, Tools, Languages and Systems used:
1. Interface: Telegram messages
2. Server Side: Linux
3. Scripting Language: Python
4. DBMS: MySQL


## Features: 
User can interact with the chatbot on telegram using intuitive commands. They are provided the following facilities  
	Details of illness : /symptoms <Illness>
This message takes in an illness and lists all the associated symptoms.
	Cure of illness/ailment : /cure <Illness>
This message takes in an ailment and shows the cure mentioned in the database.
	Scheduling Medication : /setreminder <Name of medication,
Frequency([Morning(M),Lunch(L),Dinner(D)], Number of days)>
After scheduling, the database, on the specified time,will start sending users telegram messages.

## Where does the prototype falls short : 
1.	It is short polling and hence take up a lot of resources very frequently.
2.	Due to unavailability of predefined datasets  or apis, our prototype depends on the limited database stored locally. Due to time constraints a robust database could not be created.
3.	Due to lack of required knowledge we have not been able to  stabilize the system to an acceptable level .
4.	Due to local database and its size the prototype is not very dynamic.
5.	There is no way of offline notifications.

## Possible extensions : 
1.	Using Natural Language Processing we can reduce the dependence of the bot on commands and can shift it towards the way humans usually speak. Using nltk or wit.ai we can greatly improve the user experience. Though it is also true that a command based input has less overhead and is faster.
2.	If a well compiled dataset of age, physical characteristics, symptoms and diseases is available, the product can be made very accurate on a set of a few trivial medical conditions(for which people will actually go to an app) using neural networks. It can then be used to actually customise results for individual users.
3.	A combination of the above two features can make the process of diagnostic at fingertip more intuitive and accurate. The user can ask in a very human way his concerns.
4.	A database containing diversified solutions to many trivial health problems can make the product more relevant and likeable. Creation of such a database will require extensive scrapping and surfing.
5.	Using NLP setting reminders can be made more intuitive. To obtain the best results we need to classify the intents for as many possible expressions as there are. Training is time consuming and hence has been skipped in the prototype.
6.	The product can also provide cloud storage for previous medical records for easy access.
7.	This product can be also used to connect users in remote locations to better services.



## Future Scope : 
An intuitive Chabot that communicates like humans and can provide accurate diagnoses of trivial medical conditions and first aid instructions and videos can be developed into a worthwhile product and experience. The key to stand out will be its ability to comprehend sentences and render the content in  a succinct manner.

Challenges faced and lessons learned :
1.	Training of data for NLP and NN are time consuming if not already available.
2.	We learnt how to handle json data objects in python.
3.	We learnt integratin MySQL and python
