# Zyzy 
Zyzy is a webapp that uses machine learning to estimate the value of your home in a different location.

## Table of Contents
* Overview
* Tech Stack
* Setup/Installation
* Demo
* Future Features

## Overview
Have you ever wondered how much your home would cost if it were in a different location?? well if you have, Zyzy is here for you. Zyzy is a fun web app that users can enjoy by finding out how much their home would cost if it where in a different location. The brain of the app was built using machine learning. This included a long task of exploring and wrangling data, using pandas, matplotlib and seaborn. To make the best predictions, I explored three machine leafrning algorithmns as you will see in the demo to get a better feel of each ones contribution. once the user gets to my homepage, I present to them the scope of the app(the available cities), 
they are then required to provide features of their home and also to choose a city they would like the estimate to be based off.
In return they get the estimated price of their home in their chosen city and a few general statistics will be shown using chart.js 



## Tech Stack
Data Wrangling: Pandas, Numpy , seaborn, matplotlib <br>
Framework: Flask <br>
Backend: Python, SQLAlchemy, PostgreSQL ,SciKit_Learn <br>
Frontend: Javascript , AJAX, JSON , JQuery, Jinja, HTML, CSS, Bootstrap <br>
Libraries: D3.js, chart.js

Setup/Installation
On local machine, go to desired directory. Clone  repository:

$ git clone https://github.com/Claire-Kimbugwe/House_value_estimate <br>
Create a virtual environment in the directory:

$ virtualenv env<br>
Activate virtual environment:<br>

$ source env/bin/activate<br><br>
Install dependencies:<br>
$ pip install -r requirements.txt <br>
Create database:<br><br>

$ createdb homes<br>
Build database:<br>

$ python3 -i model.py<br>
>>> db.create_all() <br>
Seed database:

$ python3 -i seed.py <br>
Run app:

$ python3 server.py <br>
Navigate to localhost:5000 in browser.


## Demo
### Data Wrangling and Exploration
I used jupyter notebook on anaconda to wrangle data and to explore trends and relations <br>
Below are a few visuals from my notebook c

![explore](/static/explore1.gif)

![explore](/static/explore3.gif)
![explore](/static/explore2.gif)<br>
![explore](/static/ML.gif)<br> <br>
### HOMEPAGE <br>
Below is muy landing page <br><br>
![home](/static/home.gif)

#### Get iformation about user's home
On this page the users provide their home features <br><br>
![features](/static/features.gif)

### Provide estimate to the users 
Here the users recieve their home estimate and a few statistics <br>
![graphs](/static/graphs.gif)


## Future Features
* utelise housing API's to get running data that will be used in training the machine learning model
* Add a login page for frequent visitors 



