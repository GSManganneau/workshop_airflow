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
- Configure pycharm or whatever u use  to point to the virtualenv: you ready to go!!!!!!

This repo contains a helper class to parse apis we are going to use for the workshop
