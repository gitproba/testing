# How to setup Teams Agent Connector

When connecting to Teams as an agent interface, please follow the guide
below.

## Step-by-step guide

1.   go to https://portal.azure.com
2.  Create a new Bot Channel Registration and enable Teams as a channel
    to use.
3.  Set the messaging endpoint for the bot channel registration to the
    following;,
    https://ag.buzzeasy.com/BuzzeasyChat/TeamsAgentConnector/api/messages/
4.  Download the custom package to your local machine.  
    1.  Within the custom package, open the manifest.json file and
        replace the "id" and "botid" with the Microsoft App ID from the
        bot channel registration created on Azure Portal
    2.  save the file and repackage into a .zip file if needed

    Teams Bot Package.zip
5.  Open Teams and go to the Team where the agent messages should arrive
    to, go to "Manage Team" -\> "Apps" and click on "Upload a Custom
    App". Select the zip package and this will be added to all channels
    within the Team.
6.  Go to the channel required for messages to arrive and get the
    channel ID. This can be retrieved from the get link feature within
    Teams and taking it from the query parameters of the URL.
7.  Add the channel ID as a destination within the desired workflow
8.  Teams Agent Connector is now ready for use.

Ensure the bot channel registration is pointing to the right environment
short name. Available short names are **DEV**, **QA**, **PRD**
