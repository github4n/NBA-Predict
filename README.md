[![Build Status](https://travis-ci.org/ConnectedMakers/NBA-Predict.svg?branch=master)](https://travis-ci.org/ConnectedMakers/NBA-Predict)

# NBA-Predict
A repository dedicated to finding and executing high percentage bets on sporting events.

We are utilizing these sites for our data.
https://stats.nba.com/

http://data.nba.net/10s/prod/v1/today.json


## Prerequisites 
```
:&   brew install python3

:&   pip3 install virtualenv

:&   git clone git@github.com:ConnectedMakers/NBA-Predict.git

:&   cd NBA-Predict

:&   python3 -m venv nba-predict

:&   source nba-predict/bin/activate

:&   pip install -r requirements.txt
```

>  To stop the python virtual environment 

    :&   deactivate

> To store installed python dependencies 

    :$   pip freeze > requirements.txt
   
Setup the google drive api
* Look at these resources for reference
    * https://gspread.readthedocs.io/en/latest/oauth2.html)
    * https://github.com/burnash/gspread
    * https://console.developers.google.com/

Save the json credentials that you will get from Google api dashboard in the project root directory like this `/NBA-Predict/client_secret.json`
* Also do not commit client_secret.json to this repo ;) 

  

## Requirements 

* Before committing locally or pushing your changes to your repo run these commands

    * Runs a python linter for source and tests
    ```
     :$   flake8 /src /test 
    ```
    * Runs unit tests
    ```
    :$    pytest
    ```

* If test or lint errors arised, then fix the errors that are given


## Getting Started 

Make sure to create a python3 virtual env. If you don't know how then refer to the prerequisites section 
the readme

Run `python src/app.py ` to invoke the main program and see results in google sheets 
