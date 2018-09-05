# workshop_airflow

# Installation
- Git clone project
- make sure python 3.6 is installed //not another version
- Make sure pip is installed or install it
- Make sure virtualenv is installed or install  with ‘pip install virtualenv’
- Create a venv in your project directory :  virtualenv -p `which python3` workshop_env
- Activate env : source workshop_env/bin/activate
- Install requirements : pip install  -r requirements.txt
- Set your project directory as  AIRFLOW_HOME variable : export AIRFLOW_HOME=PATH_TO_YOUR_PROJECT_DIRECTORY
- init the airflow project: airflow initdb
- Configure pycharm or whatever u use  to point to the virtualenv: you ready to go!!!!!!


This repo contains a helper class to parse apis we are going to use for the workshop
