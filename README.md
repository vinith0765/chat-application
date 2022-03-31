A Group video calling application using the Agora Web SDK with a Django backend.

#### 1 - Install requirements
cd mychat
pip install -r requirements.txt

#### 2 - Update Agora credentals
In order to use this project you will need to replace the agora credentials in `views.py` and `streams.js`.

Create an account at agora.io and create an `app`. Once you create your app, 
you will want to copy the `appid` & `appCertificate` to update `views.py` and `streams.js`. 

###### views.py
def getToken(request):
    appId = "YOUR APP ID"
    appCertificate = "YOUR APPS CERTIFICATE"
    ......

###### streams.js
....
const APP_ID = 'YOUR APP ID'
....

#### 3 - Start server
python manage.py runserver




