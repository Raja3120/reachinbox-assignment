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
AZURE_CLIENT_ID = ***<br>
AZURE_CLIENT_SECRET = *** <br>
AZURE_TENANT_ID = ***<br>
### Start the Server 

npm start
<br>
## Work in flow

### Starting npm 

![image](https://github.com/user-attachments/assets/b573bf1f-c36d-429e-8418-4e070cb3a940)

### Login Page

![image](https://github.com/user-attachments/assets/36d4e075-b2a8-4a4e-a77d-3ab6b6996bdf)

### Google Authentication

![image](https://github.com/user-attachments/assets/f0e8b7ce-7bcd-4b93-ba57-0fb477c4ebe4)

### Access

![image](https://github.com/user-attachments/assets/79ddac09-bc5b-43d2-b6ca-c197a66a2d7f)

### Scopes provided

![image](https://github.com/user-attachments/assets/bff86bc2-6383-4df9-8afb-582256199674)

### scopes passed

![image](https://github.com/user-attachments/assets/362e7429-968d-4605-9e24-ba18052bd0a6)

### Outlook Integration and Automated Responses

The workflow described for Google also applies seamlessly to Outlook. After connecting to an Outlook account, the application will:

1. **Parse and Check Emails:** Similar to the Google integration, it will retrieve and analyze incoming emails in the Outlook account.
2. **Automated AI Response:** The OpenAI model is employed to read the content of the emails. Based on the context, it will generate and send appropriate replies in short, concise text.

This ensures that whether you're using Google or Outlook, the application provides a consistent and efficient email management experience.










