# Go AI-Bot

## Demo

![AI-bot](https://user-images.githubusercontent.com/25595072/223883726-b23bf172-e6a6-4a7f-a441-95c0e7025537.gif)

### installation
- git clone repo
- change name of .env-example to .env
- to fill in .env:
  -

#### SLACK_APP_TOKEN (https://api.slack.com/apps)
- create a new app
- turn on socket mode
- ensure have connections:write for scope
- the token created that starts with "xapp" is the value you fill above
#### SLACK_BOT_TOKEN (https://api.slack.com/apps)
- for this you need to set OAuth on
- Bot User OAuth Token is the value you need for above
- after setting this on you will need to ensure many permissions are enabled:
  -   app_mentions:read
  - channels:read
  -  chat:write
  -  groups:history
  - im:history
  - im:read
  - im:write
  - mpim:history
  - mpim:read
  - mpim:write


#### WIT_AI_TOKEN (https://wit.ai/)
- make an account
- will need an intent, will be custom name it wolfram
- Entity go to built-in, find wit/wolfram_search_query select that
- go into Settings, there in Server access Token you will find the value of above

#### WOLFRAM_APP_ID (https://developer.wolframalpha.com/portal/myapps/)
-   once there create an account
  **note** on free acount only 2000 requests per month
  - click 'Get an AppId'
  - Fill in both app name and description
  - what is given as appId will be used to fill this column
  **caution:** there have been known errors about the delay of the creation of this IDs so one might require a 12 hour wait period before using project
