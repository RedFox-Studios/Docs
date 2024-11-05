# GitHub to Discord Notification Setup

## Objective
This guide will help you set up a **Discord webhook** to receive notifications about updates in your GitHub repositories. You’ll get notifications in a specified Discord channel for any repo events like commits, issues, pull requests, and more.

## Steps

### Prerequisites
- A **GitHub organization** with repositories.
- **Admin access** to both GitHub and Discord.
- A Discord **channel** where notifications will be sent.

---

### Step 1: Create a Webhook in Discord

1. Open **Discord** and go to the **server** where you want to set up notifications.
2. Choose the **channel** for notifications and click the **gear icon** to open channel settings.
3. Scroll to **Integrations** > **Webhooks** > **Create Webhook**.
4. Configure the webhook:
   - **Name**: Choose a descriptive name (e.g., "GitHub Updates").
   - **Channel**: Make sure it’s set to the correct channel.
5. **Copy the Webhook URL**. You’ll use this in GitHub.

### Step 2: Create a Webhook in GitHub

1. Go to your GitHub organization and open the **repository** where you want notifications.
2. Navigate to **Settings** > **Webhooks** > **Add webhook**.
3. In the **Payload URL** field, paste the **Discord Webhook URL** you copied earlier.

### Step 3: Configure the Webhook Settings

1. **Content type**: Choose `application/json`.
2. **Events**: Select which events you want to trigger notifications. Here are some common ones:
   - **Push events**: Notifies when someone pushes a commit.
   - **Pull requests**: Notifies on pull request activity.
   - **Issues**: Notifies on new or updated issues.
   - You can choose **Send me everything** for all events or pick and choose specific ones.

3. **Finish** by clicking **Add webhook**.

### Step 4: Test the Setup

1. Make a change in the GitHub repository (e.g., push a commit or open a new issue).
2. Check your Discord channel to see if the bot sent a notification. 🎉

### Step 5: Customize the Message (Optional)

The default Discord webhook message may not be fully customized, but you can use a custom bot to control the format. For full customization:
1. **Create a bot** with the [Discord Developer Portal](https://discord.com/developers/applications).
2. Use the **GitHub API** in your bot’s code to pull data from specific GitHub events.
3. Send formatted messages to the Discord channel with your bot for total control.

---

### Example Webhook Message
When configured, here’s what you might see in your Discord channel:

> **GitHub Updates**  
> 📄 New Issue Created in **repo-name**  
> 🔗 **Issue Title**: _Issue description here_  
> 🖋️ By: **Username**

---

## Troubleshooting

### Main Issues
- **No message in Discord**: Double-check the webhook URL and that GitHub events are set up correctly.
- **Permissions issues**: Ensure your Discord role has permissions to post messages in the channel.
- **Testing**: You can test your webhook directly in GitHub’s webhook settings by using **Recent Deliveries** to replay events.

### I'm getting a 400 error!

Make sure to add /github at the end of the webhook URL.

### Can I change the Avatar and Name of the hook's messages?

No, Github controls that part, so they're choosing the name and Avatar.

### I'm not getting the events I want (or too many)

Under **Which events would you like to trigger this webhook?**, select **Let me select individual events.**

Check the events you'd like to receive. There are *a lot* of them.
---

### Additional Tips

- **Multiple Repos**: Repeat the setup in each repository if you want notifications from multiple repos.
- **Custom Bot**: For a fully customized experience, consider coding a bot with GitHub API calls for advanced notifications.
