---
layout: post
title: week 8 Work Show 
Author: Jiandong Wang
comments: true
category: portfolio
tags:
    - Android 
    - Google Translate API
    - Diango REST Framework
---

This blog shows the process of our project after  Interim Presentation.



### Progress and Fixed Issues  ###

**Front-end & Back-end Comunications implemented**

First of all, we successfully connected the Android application with our server through Django REST framework and HTTP request&response.
Specially, we can show all the news from different data resources on our main page (although we will use BBC financial news as the main news stream, at the moment we just show all the news collected).
And we implemented the user register and login. We know user login is not a big deal in our project, but we got a better understanding of django RESt framework by implementing the user login.

**A few changes on Android app interface**
 
We made a fews changes on our app interface, like defining the positions of the date and news resources and discussed how to deal with news with or without pictures.

<img src="/assets/AndroidInterface.png" width="700px" />  

**More data resources adopted**

At the moment, we are collecting data from the following RSS:

* China Daily  
* BBC News  
* New York Times (new)  
* Reuters (new)  
* Sina (new)  
* People Daily (new)

But we also faced some issues in collecting news from some data resources which we decided to adopt at the very beginning of this project. I will discuss it in *Next Steps and New Issues Raise*.
<img src="/assets/RSS.png" width="700px" />  

**Translation** 

The translation has implemented by Google Translate API.  

* Not Free. Google Translate API is only available as a paid service  
* Usage Linits. Google Translate API has default limits of 2 million characters/day and 10,000 characters per 100 seconds (average 100 characters/second).  

But, Goole offer a 60 day free trial.

* Access to all Cloud Platform Products  
* $300 credit for free  
* No autocharge after free trial ends   

In addition, we are aslo trying to adopt other translate APIs and compare the translation qualities. But at this stage, Google Translate API is enough for our project.

**Encoding Issues**

We fix the encoding issue with json format and we can show the text with no garbled text on Android app now.

### Next Steps and New Issues Raise  ###

**keywords optimizing** 
For now we adopt a method from NLTK library to extract keywords from news articles. But it often produced stange words and also the accuracy is not good enough. 
We are planning to find new methods and try to overwrite them to improve the accuracy.

**Matching** 
Matching would be next step once we find a better way to extract keywords because calculating the similarities of keywords is the first step of matching based on our discussion results.

**picture positions in article**

**new encoding issues**
As I said before, when we were collecting data from some resources, like People Daily, sometimes we could get all correct text but sometimes the text we grabed was totally garbled text. 
And this issue is more serious than the encoding issue we mentioned before, which some special characters would become garbled text. We are discussing how to fix this or in the worest case we have to give up some RSS resources.
  
**new data resources needed**
At the very begining of this project, we defined some news agencies as our data resources. But when we was trying to collect the news, we found that some of them have already stopped RSS services and some xml or html structrues are too complex to analyze. 
So we have to replace those resources without update or with complex structures and we are trying to find some new news agencies as our data resources.    








