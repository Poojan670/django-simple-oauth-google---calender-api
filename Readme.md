*SETUP CREDENTIALS FOR YOUR GOOGLE APP, SCOPE AND REDIRECT ROUTES FROM google console*

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

check your access token validiting from :  https://www.googleapis.com/oauth2/v1/tokeninfo?access_token=xxxxxx

