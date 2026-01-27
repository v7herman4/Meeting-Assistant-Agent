# Installation Guide

## Table of Contents
- [Solution Overview](../README.md#overview)
- [Requirements for Installation](requirements-for-installation.md)
- [How To Use This Agent](how-to-use-this-agent.md)


### Create an App Registratio in Azure
First create an app registration in Azure.

1. Navigate to portal.azure.com
2. From the search bar, type "App Registrations" and click on the result.
3. Click on "New Registration"
4. For the "The user-facing display name for this application (this can be changed later)." , type in "Meeting Assistant Agent Registration". Leave the rest of the default items and click "Register".
5. Click on "Certificates and secrets"
6. Click "New client secret"
7. For Description enter "Meeting Assistant Agent". For Expires select "730 days".
8. From the resulting created secret, copy and paste to a notepad the "Value". Do NOT copy the "Secret ID".
9. From the left-menu click "API Permissions". Click "Add a permission". Click "Microsoft Graph". Click "Delegated permissions". 
10. In "Select permissions", type in Calendars.Read, select the entry and click "Add permissions".
11. Repeat the for the following:
- offline_access
- OnlineMeetings.Read
- OnlineMeetingTranscript.Read.All
12. Make sure to "Grand admin consent" for each item. The result should look like below:

