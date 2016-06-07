---
layout: post
title: Run context4news project 
comments: true
category: portfolio
tags:
    - djiango
    - postgres
---

There is an example with Django apps, e.g., reading news articles from RSS feeds and streaming tweets.
This blog is about how to run this example project. How to get the news and display them. 

### Clone the project from github  ###
Using the following command to clone this reposity:

git clone git@github.com:ucd-nlmsc-teamproject/context4news.git

Then we got the example. 

###  Configure Postgresql ###

We get the newsdb.dump from Georgiana.
First we need to create a new database named newsdb.
create newsdb
Then within the folder where you copied the database dump run:
psql -U postgres -d newsdb < newsdb.dump

The tables are :
<img src="/assets/newsdb.jpg" width="700px" />

And we can check the information in the table "articles_article":
<img src="/assets/article.jpg" width="1000px" />

### Edit Function file ###
This project can get the news from RSS Feeds. First we need to edit funciton.py file based on the news html. Because different 
websites might use differents tags/class in their html.
<img src="/assets/function.jpg" width="700px" />


### Data collecFon ###

Repeated jobs (cron like jobs): arFcles/tasks.py
(Needs Redis + Celery)
pip install redis
redis-server &
<img src="/assets/redis.jpg" width="700px" />

python manage.py celeryd -l info -B -c 5
<img src="/assets/collection.jpg" width="700px" />

### Run ###

Within the folder where you project is run:
python manage.py runserver

Then we can get the result:
<img src="/assets/newapp.jpg" width="1000px" />



