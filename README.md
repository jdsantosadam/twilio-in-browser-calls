# Making and Receiving Phone Calls from the Browser with Twilio Programmable Voice, Python and JavaScript

## Requirements

- Python 3.10.x
- [Twilio Account](https://www.twilio.com/try-twilio)
- Tunneling service like [ngrok](https://ngrok.com/)


## About the project

This project is able to make and receive phone calls from the browser using Twilio Programmable Voice and the Twilio Python SDK.
The source and the base documentations can be found below:
- [Make and Receive Phone Calls from the Browser with Twilio Programmable Voice, Python and JavaScript](https://www.twilio.com/blog/make-receive-phone-calls-browser-twilio-programmable-voice-python-javascript)

Follow along the docs to get the project up and running.

With all of these configured, make the call from the browser (or from a phone to the Twilio number).

## How to run

Configure the project according to the documentation above. Run the Flask server, and then tunnel the port using ngrok and copy the URL. Then, configure the Twilio App with the URL and attach the Twilio App to a Twilio number (see the documentation above).

With the application running, access the localhost URL in the browser and make a call to the Twilio number.

```shell
python main.py

# access the localhost URL in the browser 
# localhost:3000

# In another terminal
ngrok http 3000
```

## Using in conjunction with the Twilio Media Stream project

Call the configured number that has the attached TwiML Bin that will send the audio stream to this Flask server. The transcription will be printed in that project console.

Remember, run this project and the Twilio Media Stream project in different terminals.


