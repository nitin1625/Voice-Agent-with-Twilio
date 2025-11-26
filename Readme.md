# Voice Agent

This project implements a minimal voice agent using Deepgram and Twilio. It follows the basic structure and workflow described in the Deepgram documentation.

## Requirements

* Python 3.10+
* Virtual environment
* Deepgram API key
* Twilio account credentials

## Setup

1. Create and activate a virtual environment:

   ```
   python -m venv venv
   source venv/bin/activate    # Linux/Mac
   venv\Scripts\activate       # Windows
   ```

2. Install dependencies:

   ```
   pip install -r requirements.txt
   ```

3. Create a `.env` file and add required credentials:

   ```
   DEEPGRAM_API_KEY=[your key]
   TWILIO_ACCOUNT_SID=[your sid]
   TWILIO_AUTH_TOKEN=[your token]
   ```

4. Update `json.config` if required for your Twilio webhook configuration.

## Running the Application

Start the server:

```
python main.py
```

Expose your local server if necessary:

```
ngrok http 5000
```

Use the generated URL as the Twilio Voice webhook.

## File Structure

* `main.py` – application entry point
* `json.config` – configuration for webhook and routing
* `.env` – environment variables
* `.gitignore` – git ignore rules
* `Readme.md` – project overview

## Reference

Deepgram + Twilio Voice Agent documentation:
[https://developers.deepgram.com/docs/twilio-and-deepgram-voice-agent](https://developers.deepgram.com/docs/twilio-and-deepgram-voice-agent)
