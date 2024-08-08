### Overview
This server-based application, built with Node.js and Express, manages and automates email responses for Google and Outlook accounts. By leveraging BullMQ as a task scheduler, the server parses incoming emails, uses AI to analyze the context, and responds accordingly. This project integrates multiple services and APIs to provide a seamless and intelligent email management experience.

### Technologies Used
Node.js
Express.js
OpenAI
Google APIs
Microsoft Graph API

### NPM Packages
dotenv - For environment variable management.
axios - For making HTTP requests.
bullMQ - For task scheduling and queue management.
google-auth-library - For Google OAuth2.0 authentication.
ioredis - Redis client for Node.js.
@microsoft/microsoft-graph-client - Microsoft Graph API client.
@azure/msal-node - Microsoft Authentication Library (MSAL) for Node.js.

### Environment Variables
Create a .env file in the root directory with the following keys (refer to the API documentation for specific values):

PORT = ***

GOOGLE_CLIENT_ID = ***
GOOGLE_CLIENT_SECRET = ***
GOOGLE_REDIRECT_URI = ***
GOOGLE_REFRESH_TOKEN = ***
OPENAI_SECRET_KEY = ***
redis_port = ***
redis_host = ***
redis_pass = ***
AZURE_CLIENT_ID = ***
AZURE_CLIENT_SECRET = *** 
AZURE_TENANT_ID = ***

### Start the Server 

npm start

