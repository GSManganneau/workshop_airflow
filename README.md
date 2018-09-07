# workshop_airflow

# prerequisites
- Python 3.6 
- pip (packagement management for python)
- virtualenv ( pip install virtualenv)
- virtualbox 
# Installation

```
git clone git@github.com:GSManganneau/workshop_airflow.git
```

```
cd workshop_airflow
```

Create a venv in your project directory :  
```
virtualenv -p `which python3` workshop_env
```
Activate env : 
```
source workshop_env/bin/activate
```

Install requirements : 
``` 
pip install  -r requirements.txt
```

Set your project directory as  AIRFLOW_HOME variable : 
```
export AIRFLOW_HOME=$( pwd )
```

init the airflow project: 
```
airflow initdb
```

This repo contains a helper class to parse apis we are going to use for the workshop.
To use it, add the utils directory to your python path. Add the following line to your bash profile and source it:
```
export PYTHONPATH="${PYTHONPATH}:/my/utils/directory"
```

To access APIs you will need to create "connections" in the airflow DB
- First connection
```
connection id: navitia
host: https://api.navitia.io/v1/coverage/fr-idf/
connection type: http
```
In the Operator instance, add these arguments:
```
endpoint='journeys?from=2.2728894%3B48.8812988&to=2.2950275%3B48.8737917&',
headers={'Authorization': '9cdfa8dd-4ed8-4411-a6eb-690d361fddf6'}
```
- Second connection
```
connection id: weather_api
host: http://api.apixu.com/
connection type: http
```
In the Operator instance, add this argument:
```
endpoint='v1/current.json?key=c285ac3bd7f84e88904144311182808&q=Paris'
```

For the SMTP server, either:
- set up your own (in the airflow.cfg file)
- use the login/password defined in the Openvalue Slack Channel "workshop"

Configure pycharm or whatever u use  to point to the virtualenv: you ready to go!!!!!!

