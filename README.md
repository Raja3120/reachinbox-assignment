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

## Working flow

<br>

### Starting npm 

<br>

![image](https://github.com/user-attachments/assets/b573bf1f-c36d-429e-8418-4e070cb3a940)
<br>

### Login Page

<br>

![image](https://github.com/user-attachments/assets/36d4e075-b2a8-4a4e-a77d-3ab6b6996bdf)
<br>

### Google Authentication
To enable Google authentication, set up OAuth 2.0 credentials in the Google Cloud Console by creating a new project and configuring your OAuth consent screen. Download the OAuth credentials file and store the client_id, client_secret, and redirect_uri in your .env file. Ensure that the necessary API scopes are added for reading, sending, and modifying Gmail emails.

<br>

![image](https://github.com/user-attachments/assets/6419b979-5726-419f-9942-6f97c4ba8011)


<br>

### Access

For enabling Google access, users will typically see a consent screen during the OAuth process, where they can choose to either "Continue" or "Cancel". The "Continue" option grants the specified permissions (such as reading, sending, and modifying emails), while "Cancel" will deny access, and the application will not be able to interact with the user's Google account. Make sure your application clearly explains the permissions it requires and why they are necessary to ensure user trust and compliance with Google's policies.
<br>

![image](https://github.com/user-attachments/assets/d915a582-181e-4315-b910-de916ec2f7dc)

<br>

### Scopes used
1. **Read**: Accesses the user's email messages and metadata for analysis and processing.
2. **Write**: Allows modification and updating of email messages, such as organizing or tagging.
3. **Send**: Grants permission to send emails on behalf of the user, essential for automating responses.

These scopes enable full email management capabilities, including reading, organizing, and sending messages.


<br>

![image](https://github.com/user-attachments/assets/ba40ed0f-dc5a-4c18-96ea-4375e85895bd)

<br>

### scopes passed

<br>

![image](https://github.com/user-attachments/assets/362e7429-968d-4605-9e24-ba18052bd0a6)

### Outlook Integration and Automated Responses

The workflow described for Google also applies seamlessly to Outlook. After connecting to an Outlook account, the application will:

1. **Parse and Check Emails:** Similar to the Google integration, it will retrieve and analyze incoming emails in the Outlook account.
2. **Automated AI Response:** The OpenAI model is employed to read the content of the emails. Based on the context, it will generate and send appropriate replies in short, concise text.

This ensures that whether you're using Google or Outlook, the application provides a consistent and efficient email management experience.

### Demonstration

To showcase the tool's functionality:

1. **Connect Email Accounts**: Use OAuth to connect new email accounts for both Gmail and Outlook.
2. **Send Test Emails**: Send an email to these accounts from another account to generate test data.
3. **Email Processing**: The tool will read the incoming emails, categorize them, and assign labels accordingly.
4. **Automatic Reply**: Display the automatic reply sent based on the content of the received emails.

This demonstration highlights the tool's capabilities in managing and responding to emails efficiently.









