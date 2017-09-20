Python Retweet Bot
==================

![alt text](https://img.shields.io/badge/python-3.5-green.svg "Python3.5")

This script retweets all Tweets containing your search term. To limit Twitter
requests a savepoint file marks Tweets found before. It's Twitter API v1.1 ready. The configuration files are stored as 
```.yml``` files, and an example ```twitter_config.yml``` file is included for the sake of completeness.

Dependecies:
-------------
* Tweepy
* PyYaml

```pip install -r requirements.txt```

How to start:
-------------

* Define your hashtag or search query in the config file
* Define the number of Retweets at a time (This avoids overloading -Limit is 180 RT/ 15 mins)
* Add your Twitter app credentials in the config file
* (Tune some other options if you like)
* $ python retweet.py
* It will be killed when you turn off your machine, so either install on a RPi or...
* Use the Procfile to run it on Heroku

Compatibility
-------------

Compatible with Python 3.x ,tested  on Python 3.5.
