# Provision a new tenant

In order to setup a new tenant on the Buzzeasy Chat Service, the tenants
services need to be created using the step by step guide below. All
tenants have their own service within Buzzeasys cloud including
storages, Service Fabric applications, key vaults etc. This guide will
go through the entire setup to get a tenant up and running and ready to
go-live.

## Pre-Requisites

-   Access to Visual Studio Team Services and permissions to
    build/release
-   Access to Azure Portal to create resources (when required)
-   Virtual Machine on premise to install a cloud connector if Hybrid
    Environment (Skype for Business only)
-   Access to Buzzeasy Portal with super admin rights to create company 

## Step-by-step guide

**Steps**

1.   Login to the Buzzeasy Portal and create a company with the tenants
    name
2.  Setup a Chat Service as per the article within the chat service
    section. once this has been completed, make note of the chat service
    ID as this will be needed later in the setup  
3.  Login to VSTS (Visual Studio Team Services) and navigate to Build /
    Release page for the Buzzeasy Project
4.  Edit the Release Definition for BuzzeasyChat Tenant ARM
5.  Add a new Environment with an empty process and name it after the
    tenant
6.  Add an agent task of ARM tenant deployment to PROD
7.  Set the CustomerName to the Tenant ShortCode
8.  Save the Release
9.  Open the BuzzeasyChat Tenant ARM releases and queue a new release
10. Press Deploy to the customers environment
11. Add a bot channel for the customer facing integration. Set the
    messaging endpoint of the bot channel to be
    https://chat.buzzeasy.com/BuzzeasyChatXXX/BotFrameworkConnector/api/messages/
12. Enable the required channels e.g. Facebook , Skype, Web Chat, Direct
    Line etc. for the customer connector
13. Add a bot channel for agent teams integration.
14. Set the messaging endpoint of the bot channel to be
    https://chat.buzzeasy.com/BuzzeasyChatXXX/TeamsAgentConnector/api/messages
15. Enable Teams as a channel on the bot channel registration
16. 17. 
