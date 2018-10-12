# disastaware
Spreading natural disaster awareness throughout the cyberspace


## Purpose of the program

* Spread awareness about any ongoing or recently occurred natural disaster through social media — for now only Twitter.
* Possibly make the public empathize with the victims, by tailoring the message to their individual personality.
* And thus, try to maximize help and donations from the public to the rescue efforts.

## What will the app do

The app will try to target people who are either unaware of the disastrous situation completely or are having incomplete or less than enough knowledge of it. This can be done using graph search methods, the graph being the social graph of that social media, eg. for Twitter it will be the graph with all the users as nodes and the follower and following relations as edges. For every node, the app will evaluate a "score" of the node, the score being an indicator of the user knowing about the disastrous situation adequately. If the score is below a certain threshold, the app will make a post towards that person, containing information about the disaster, trying to make them empathize, and letting them know how they can help. This way, the app won't "spam" people who already know about the situation.

For the app to be considered effective and successful, the following two aspects would be most crucial:

* __Calculating the _score___: For calculating the score, various machine learning and NLP techniques and possibly Azure APIs would be used on the user's recent activities. For example, if the user has recently tweeted or retweeted about the disaster recently, that means he very likely knows about the situation already.

* __Searching the graph__: One of the most important goals of this program is spreading awareness and letting as many people as possible. As we have limited resources — computing power, API consumption rate, time — the program will have to be careful not to search redundantly among people with very little success, success being finding and informing an uninformed person. That means employing a very sophisticated graph search technique. This technique should give lower priority to subgraphs // subtrees where the leading node already knows about the situation and has tweeted about it, because that would mean his followers most likely have already seen his tweet, and therefore they know about the situation too.

* __Getting information about natural disasters__: The app would constantly check some trustable sources for any updates regarding any natural disaster that may be happening. Whenever it finds a new disaster, it would get to work. It would look up as much information as it can about it online, and then use that corpus of information to create the messages // tweets. 

* __Personalizing the message for every user__: The app would try to make a psychological profile of the user by analyzing his previous activities, using Azure psychometric APIs. Taking that information, the app would try and craft personal messages for every individual user, so that the message touches him and makes him empathize. 


All of this would be done automatically, no human interaction would be needed. The app would get to work automatically as soon as any natural disaster occurs.
