#Getting started with Twilio Video for Web in Python

Following tutorial at https://www.twilio.com/docs/api/video/quickstart-sample-apps.

Fork Twilio demo https://github.com/TwilioDevEd/video-quickstart-python.

####Install twilio-video javascript SDK, Chrome and Firefox are supported 
```npm install --save twilio-video```

####Setup Info
Config Value | Description
-------------------------- | --------------------------
Configuration Profile SID | Identifier for a set of config properties for your video application
Account SID | Your primary Twilio account identifier
API Key | Used to authenticate
API Secret | Used to authenticate

Python server application uses [Flask](http://flask.pocoo.org/).

####Setup application

Begin by creating a configuration file for your application:

```bash
cp .env.example .env
```

Edit `.env` with the four configuration parameters we gathered from above. 

Next, we need to set up your Python environment. Install `virtualenv` via `pip`:

```bash
pip install virtualenv
```

Next, we need to install our depenedencies:

```bash
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```

Now we should be all set! Run the application using the `python` command.

```bash
python app.py
```

Your application should now be running at [http://0.0.0.0:5000](http://0.0.0.0:5000). Select any room name and join the room. Join the same room with another user in another browser tab or window to start video chatting! When you're finished, deactivate your virtual environment using `deactivate`.

![screenshot of chat app](https://s3.amazonaws.com/com.twilio.prod.twilio-docs/images/video2.original.png)
