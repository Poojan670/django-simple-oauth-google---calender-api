*SETUP CREDENTIALS FOR YOUR GOOGLE APP, SCOPE AND REDIRECT ROUTES FROM google console*
**ENABLE GOOGLE CALENDER API IN ENABLED APP& SERVICES**
**setup OAUTH Consent screen, and add your desired scopes**
if the app is unpublished, add your testing mail to test users

ADD your domain to Authorised JavaScript origins

ADD your redirect urls to Authorised redirect URIs


**SETUP .ENV SIMILAR TO .ENV.SAMPLE**

**GET CLIENT_ID AND CLIENT_SECRET FROM GOOGLE CREDENTIALS**

->Download .json file and put it in the project directory, rename it to credentials.json

setup a virtual env

-> venv/Scripts/activate

pip install -r requirements.txt

py manage.py migrate

py manage.py runserver 8000

**ENJOY**


***Additional Info***
Calender Insufficient Permission might occur due to lack of given scopes as needed or lack of scopes in your respective google app 
    additional help -> make sure calender api is enabled in google cloud console
                    try removing your app access in your https://myaccount.google.com/permissions, this will make you re authorize your app access to your gmail

**Changes made in cloud console can take upto 2-10 mins**


check your access token validiting from :  https://www.googleapis.com/oauth2/v1/tokeninfo?access_token=xxxxxx

