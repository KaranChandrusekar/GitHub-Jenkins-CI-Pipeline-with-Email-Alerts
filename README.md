**GitHub-Jenkins-CI-Pipeline-with-Email-Alerts**

This project demonstrates a simple Jenkins pipeline: (Attached screenshot of my execution with this repo)

- Triggers automatically on GitHub commits via webhooks.
- Clones the repository and executes a build.
- Sends email notifications for build success/failure.

**Setup Instructions**
1. Jenkins Configuration
- Configure Email Notifications : Go to Manage Jenkins > Configure System .
- Under Extended E-mail Notification : Set SMTP Server : smtp.gmail.com (for Gmail).
- Enable Use SMTP Authentication and provide credentials.

2. GitHub Webhook Setup
 - Go to your GitHub repository:
 - Navigate to Settings > Webhooks > Add Webhook.
 - Payload URL : http://<JENKINS-URL>/github-webhook/.
 - Trigger : Select Just the push event.
 - Save the webhook.

3. Jenkins Pipeline Configuration
 - Create a new pipeline in Jenkins
 - For exact script, refer my screenshot.

4. Pipeline Output Example
 - On successful execution, you’ll receive an email like my email output screenshot
 - Check your spam, if not received.

 
