# workshop_airflow

#Installation
- Git clone project
- make sure python 3.6 is installed //not another version
- Make sure pip is installed or install it
- Make sure virtualenv is installed or install  with ‘pip install virtualenv’
- Create a venv in your project directory :  virtualenv -p `which python3` workshop_env
- Activate env : source workshop_env/bin/activate
- Install requirements : pip install  -r requirements.txt
- Set your project directory as  AIRFLOW_HOME variable : export AIRFLOW_HOME=PATH_TO_YOUR_PROJECT_DIRECTORY
- init the airflow project: airflow initdb
- Set smtp server in airflow.cfg :
    - [smtp] If you want airflow to send emails on retries, failure, and you want to use the airflow.utils.email.send_email_smtp function, you have to configure an smtp server here
    - smtp_host = smtp.sendgrid.net
    - smtp_starttls = True
    - smtp_ssl = False
    - # Uncomment and set the user/pass settings if you want to use SMTP AUTH
    - smtp_user = azure_a7f0605203ef91d605d64e0d7fab9351@azure.com
    - smtp_password = Z&"3Wj7AycXyBkN8/J7#y;n;nJ/y7@snH#9F+~?Ht5eDaGSFKD
    - smtp_port = 587
    - smtp_mail_from = themailyouwant@whatever.com
- Configure pycharm or whatever u use  to point to the virtualenv: you ready to go!!!!!!

This repo contains a helper class to parse apis we are going to use for the workshop
