### Overview
This server-based application, built with Node.js and Express, manages and automates email responses for Google and Outlook accounts. By leveraging BullMQ as a task scheduler, the server parses incoming emails, uses AI to analyze the context, and responds accordingly. This project integrates multiple services and APIs to provide a seamless and intelligent email management experience.

### Technologies Used
Node.js<br>
Express.js<br>
OpenAI<br>
Google APIs<br>
Microsoft Graph API<br>
### NPM Packages
dotenv - For environment variable management.<br>
axios - For making HTTP requests.<br>
bullMQ - For task scheduling and queue management.<br>
google-auth-library - For Google OAuth2.0 authentication.<br>
ioredis - Redis client for Node.js.<br>
@microsoft/microsoft-graph-client - Microsoft Graph API client.<br>
@azure/msal-node - Microsoft Authentication Library (MSAL) for Node.js.<br>
### Environment Variables
Create a .env file in the root directory with the following keys (refer to the API documentation for specific values):<br>
PORT = ***<br>
GOOGLE_CLIENT_ID = ***<br>
GOOGLE_CLIENT_SECRET = ***<br>
GOOGLE_REDIRECT_URI = ***<br>
GOOGLE_REFRESH_TOKEN = ***<br>
OPENAI_SECRET_KEY = ***<br>
redis_port = ***<br>
redis_host = ***<br>
redis_pass = ***<br>
AZURE_CLIENT_ID = ***<br>
AZURE_CLIENT_SECRET = *** <br>
AZURE_TENANT_ID = ***<br>
### Start the Server 

npm start

