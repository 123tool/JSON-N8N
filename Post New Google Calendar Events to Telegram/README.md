Prerequisites
Before setting up the workflow, ensure the following:

Google Account with Google Calendar Access: The Google Calendar API must be enabled.
Telegram Bot: Create a bot using BotFather on Telegram.
Telegram Chat ID: Retrieve the Chat ID (personal chat or group).
Use OAuth2 for Google Calendar and a Bot Token for Telegram.
Steps
Step 1: Google Calendar Trigger Node (Event Created Event)
Click "Add Node" and search for Google Calendar.
Select "Google Calendar Trigger" and add it to the workflow.
Authenticate with your Google Account.
Select "Event Created" as the trigger type.
Choose the specific calendar to monitor.
Click "Execute Node" to test the connection.
Click "Save".
Step 2: Telegram Node (Send Message Action)
Click "Add Node" and search for Telegram.
Select "Send Message" as the action.
Authenticate using your Telegram Bot Token.
Set the Chat ID (personal or group chat).
Format the message using details from Google Calendar Trigger and set the message in text.
Click "Execute Node" to test.
Click "Save".
Step 3: Connect & Test the Workflow
Link Google Calendar Trigger → Telegram Send Message.
Execute the workflow manually.
Create a test event in Google Calendar.
Check Telegram to see if the event details appear.
n8n Workflow Created by WeblineIndia
This workflow is built by the AI development team at WeblineIndia. We help businesses automate processes, reduce repetitive work, and scale faster.

Need something custom? You can hire AI developers to build workflows tailored to your needs.
