# slack-thread-response-bot

## Usage

- Install dependencies with `pipenv install`
- Create a Slack app, install it into a workspace, and add it to a channel
- Create a .env file with SLACK_OAUTH_TOKEN and MESSAGE_FILE_NAME set (the latter controls the text file where the Bot's message is persisted)
- Run the API server via `pipenv run uvicorn main:app --host <local IP> --reload`
- Use [ngrok](https://ngrok.io) to tunnel connections to the port the API is served on
- Add the public URL to the Events API redirect URL, and subscribe to channel messages
- Use the root web page to edit the message the bot replies with
