# jess-channel-invite-test-app
Main test app for working with Bolt.

# How To Use
1. Create a Slack app with `chat:write`, `channel:read`, `group:read`, and `commands` scopes.
2. Install your Slack app to generate token.
3. Create a .env file in the root of the app folder and add the following lines, replacing the secret and token as needed:
```
SLACK_SIGNING_SECRET="Enter-Your-Real-Signing-Secret-Here"
SLACK_BOT_TOKEN="Enter-Your-Real-Bot-Token-Here"
```
4. Add member_joined_channel event listener in Event Subscriptions
5. Add a /create slash command to your app and direct it to your app.
6. Call your slash command from a channel and provide the information requested to create a channel and invite a default user.
