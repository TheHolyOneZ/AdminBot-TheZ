# AdminBot Features Documentation

AdminBot is a comprehensive and robust Discord bot designed to manage and enhance server experiences. Below is a detailed feature breakdown, comparing AdminBot to popular alternatives like MEE6, Dyno, and Carl-Bot.


#### If u want the sourcecode feel free to dm me on discord or just open a ticket wiith the command "!ticket AdminBot" 
[![Discord](https://img.shields.io/badge/Join%20our%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/zsGTqgnsmK)




| Feature                                | AdminBot | MEE6 | Dyno | Carl-Bot |
|----------------------------------------|----------|------|------|----------|
| **Moderation Commands**                | ✅        | ✅    | ✅    | ✅        |
| - Ban/Kick/Warn                        | ✅        | ✅    | ✅    | ✅        |
| - Clear Messages                       | ✅        | ✅    | ✅    | ✅        |
| - Mute with Duration                   | ✅        | ❌    | ✅    | ✅        |
| **Advanced Logging**                   | ✅        | ❌    | ❌    | ✅        |
| - Action Logging (Bans, Mutes, etc.)   | ✅        | ❌    | ❌    | ✅        |
| - Ticket Transcript Logging            | ✅        | ❌    | ❌    | ✅        |
| **Ticket System**                      | ✅        | ❌    | ❌    | ✅        |
| - Button-based Claim and Close         | ✅        | ❌    | ❌    | ✅        |
| - Add/Remove Users in Tickets          | ✅        | ❌    | ❌    | ✅        |
| - Ticket Logs                          | ✅        | ❌    | ❌    | ✅        |
| **Server Management Tools**            | ✅        | ✅    | ✅    | ✅        |
| - Lockdown/Unlock Channels             | ✅        | ✅    | ✅    | ✅        |
| - Slowmode Configuration               | ✅        | ❌    | ✅    | ✅        |
| - Announcement Command                 | ✅        | ❌    | ✅    | ✅        |
| **Dynamic Status Updates**             | ✅        | ❌    | ❌    | ❌        |
| - Rotating Status Messages             | ✅        | ❌    | ❌    | ❌        |
| - Status Reflecting Server Stats       | ✅        | ❌    | ❌    | ❌        |
| **Custom Commands**                    | ❌    | ❌    | ✅    | ✅        |
| **Embed Message Customization**        | ✅        | ❌    | ❌    | ✅        |
| - Customizable Colors and Fields       | ✅        | ❌    | ❌    | ✅        |
| **Role Management with Panels**        | ✅        | ❌    | ❌    | ✅        |
| - Reaction-based Role Assignment       | ✅        | ❌    | ❌    | ✅        |
| **Welcome System (Highly Configurable)**| ✅        | ❌    | ❌    | ✅        |
| - Placeholders for User/Server Details | ✅        | ❌    | ❌    | ✅        |
| - Configurable Welcome Message         | ✅        | ❌    | ❌    | ✅        |
| **Auto-Moderation**                    | ✅        | ❌    | ✅    | ✅        |
| - Caps/Spam/Banned Word Detection      | ✅        | ❌    | ✅    | ✅        |
| - Configurable Thresholds              | ✅        | ❌    | ✅    | ✅        |
| **Activity and Member Tracking**       | ✅        | ❌    | ❌    | ❌        |
| - Server/Member Stats                  | ✅        | ❌    | ❌    | ❌        |
| - User Information Commands            | ✅        | ❌    | ❌    | ❌        |
| **Free and Open Source**               | ✅        | ❌    | ❌    | ❌        |
| **Pricing**                            | Free     | Freemium | Freemium | Freemium |
| **Custom Invite Links**               | ✅        | ❌    | ❌    | ❌        |
| **Full Server Backup**                 | ✅        | ❌    | ❌    | ❌        |
| **Full Config Backup**                 | ✅        | ❌    | ❌    | ❌        |
| **Owner Panel**     | ✅        | ❌    | ❌    | ❌        |

--- 
## Detailed Feature Breakdown

### 1. Moderation Commands
AdminBot provides a full suite of moderation tools to keep your server safe:
- `!ban <user> [reason]`: Permanently ban a user.
- `!kick <user> [reason]`: Remove a user from the server.
- `!mute <user> <duration> [reason]`: Temporarily mute a user with a specified duration.
- `!warn <user> [reason]`: Issue warnings to members.
- `!clear <amount>`: Bulk delete messages in a channel.
- `!nuke`: Completely cleans a channel.
- `!vcmute <user>`: Mutes a user in a voice call.
- `!vcunmute <user>`: Unmutes a user in a voice call.

### 2. Advanced Logging
Keep track of server activities with detailed logs:
- Moderation actions such as bans, kicks, mutes, and warnings are logged.
- Ticket logs, including transcripts, are automatically saved in a dedicated `#ticket-logs` channel.

### 3. Ticket System
AdminBot offers a robust ticketing system for user support:
- Button-based interaction for claiming and closing tickets.
- Add or remove users dynamically to collaborate on resolving issues.
- Automatic logging and transcription of ticket discussions.

### 4. Server Management Tools
Enhance server management with powerful tools:
- `!lockdown [channel] [duration]`: Restrict sending messages in a channel, now with optional duration.
- `!unlock [channel]`: Reopen a previously locked channel.
- `!slowmode <seconds>`: Set a cooldown between messages.
- `!announce <color/hex code> <channel> <message>`: Create a server announcement. If links are included, the bot will create a separate overview of the links.
- `!massrole <role>`: Adds a specific role to all users on the server at once.

### 5. Dynamic Status Updates
Keep your server engaged with rotating status updates:
- Customizable status messages reflecting server stats like member count and activity.

### 6. Role Management
Streamline role assignment with:
- Reaction-based role panels for self-assignment.
- Commands like `!addrole <user> <role>` and `!removerole <user> <role>` for admins.

### 7. Welcome System
Customize user onboarding:
- Placeholders like `{user}`, `{server}`, and `{count}` allow personalized welcome messages.
- Commands to configure the color, channel, and content of welcome messages.

### 8. Auto-Moderation
Ensure a safe environment with automated moderation:
- Detection of caps, spam, and banned words with configurable thresholds.
- Flexible settings to suit different server needs.
- Enhanced `!automod spam_threshold` with custom timeout durations for spamming.

#### Automod Commands:
- `caps_threshold`: Configure the tolerance for caps in messages.
- `spam_threshold`: Set the number of repeated messages to trigger spam detection.
- `spam_interval`: Define the time window for spam detection.
- `banned_words`: Add or remove words for automated filtering.
- `link_whitelist`: Manage a list of allowed links.

#### Usage:
- `!automod <configuration> <value>`
#### Example:
- `!automod caps_threshold 5`
- `!automod spam_threshold 4 10` (4 messages allowed within 5 seconds; 10-second timeout)
- `!automod banned_words BADWORD`
- `!automod link_whitelist https://www.example.com`

### 9. Information and Analytics
Gain insights into server and user activity:
- `!serverinfo`: Display server stats like member count and creation date.
- `!userinfo [user]`: Retrieve detailed information about a user.
- `!roles`: List all server roles and their member counts.
- `!stats`: Show bot statistics including uptime and server count.
- `!servericon`: Displays the server icon in full size.
- `!avatar <user>`: Displays a user's avatar in full size.
- `!ping`: Shows the bot's response time.

### 10. Polls and Embeds
Create engaging content:
- `!poll`: Creates a reaction-based poll.
- `!embed`: Creates a custom embed message.
- `!say <message>`: Makes the bot send a message.

### 11. Full Server Backup and Restore
Ensure the safety of your server's configuration and content:
- `!backup`: Creates a full backup of the server, including channels, roles, server settings, attachments, and messages/emojis.
- `!restore <backup_file>`: Restores the server to a previously backed-up state.

### 12. Full Config import and export
Included Settings
• Welcome System
• Ticket System
• AutoMod
• Role Management
• Server Management
- `!export`: Exports the entire bot configuration as a JSON file.
- `!import <json_file>`: Imports a configuration from a JSON file.
- 
### 13. MiniGames
- `!numbergame <number> <channel>`: Lets admins create a number game.
- `<number>`: If nubmergame started players can enter numbers in the channel it started to guess it.
- `!tictactoe`: lets u start a tictactoe game.

Easy to use will give a announcement in the channel where game was started and a win announcement when someone wins.

### 14. Owner Panel
 - `!owner`: Opens a panel for owner-only commands.
 - `!executecmd <guild_id> <channel_id> <command>`: Execute commands in other servers
 - `!leaveserver <guild_id>`: Make bot leave a specific server
 - `!botinfo`: View detailed bot statistics
Also if u do !owner it will give you a panel with interactive buttons like Statics and server lists

### 15. Custom Invites
- `!invite <duration> <max uses>`: Create an invite link for a channel with customizable duration and max uses
- `!invite_view`: Show all invite links and information about them

  
Usage Example: `!invite 32 21` 

output: 

![image](https://github.com/user-attachments/assets/fbd3812f-7c81-403c-9a3b-3bfdda627a88)

---

## Complete Command List

### Moderation Commands
- `!ban <user> [reason]`
- `!kick <user> [reason]`
- `!mute <user> <duration> [reason]`
- `!warn <user> [reason]`
- `!clear <amount>`
- `!nuke`
- `!vcmute <user>`
- `!vcunmute <user>`
- `!nickname <user_id> <nickname>`

### Server Management Commands
- `!lockdown [channel] [duration]`
- `!unlock [channel]`
- `!slowmode <seconds>`
- `!announce <message>`
- `!massrole <role>`
- `!addrole <user> <role>`
- `!removerole <user> <role>`
- `welcome`: Lets you configure the welcome message, color, and channel.

### Ticket System Commands
- `!ticket [reason]`
- `!add <user>`
- `!remove <user>`
- `!close`
- Includes clickable elements to claim or close a ticket.

### Information Commands
- `!serverinfo`
- `!userinfo [user]`
- `!roles`
- `!stats`
- `!servericon`
- `!avatar <user>`
- `!ping`

### Automod Configuration
- `caps_threshold`
- `spam_threshold`
- `spam_interval`
- `banned_words`
- `link_whitelist`

### Polls and Embeds
- `!poll`
- `!embed`
- `!say <message>`

### Backup and Restore
- `!backup`
- `!restore <backup_file>`

### Config import and export
- `!importconfig <config_file>`
- `!exportconfig` 

### MiniGames
- `!numbergame <number> <channel>`: Lets admins create a number game.
- `<number>`: If nubmergame started players can enter numbers in the channel it started to guess it.
- `!tictactoe`: lets u start a tictactoe game.
  
### Custom Invites
- `!invvte <duration> <max uses>`: Create an invite link for a channel with customizable duration and max uses
- `!invite_view`: Show all invite links and information about them

---

With all these features, AdminBot ensures a comprehensive management experience. Plus, it includes over 1600+ banned words in its default automod configuration, ensuring safety and compliance. And you know what’s crazy? It’s entirely free and open source.

Made by TheZ



## GUIDE

# How to Set Up Bot Permissions in Discord

## 1. Create Roles for Your Bot

To ensure your bot functions as needed, you need to create at least two roles:
- **Bot Role (Top Hierarchy)**: This role will have all the necessary permissions for the bot to interact with the server. This role should be at the **top of the role hierarchy**.
- **Secondary Role (Lowest Hierarchy)**: This role will be optional for the bot and is mainly for organizational purposes. It won't grant any permissions but can be placed **anywhere in the member list** (e.g., above owner, below admin, or below members) depending on your preference.

## 2. Setting Up the Bot Role

- **Step 1**: Go to **Server Settings** > **Roles**.
- **Step 2**: Click on the **+** (Create a New Role) button to add a new role.
- **Step 3**: Name this role something like "Bot" or "Bot Permissions".
- **Step 4**: Assign **all permissions** that the bot needs to function (e.g., **Manage Messages**, **Send Messages**, **Manage Roles**, **Administrator**).
- **Step 5**: Place this role **at the top of the hierarchy**. This ensures that the bot can manage other roles and messages. To do this:
  - Under the **Roles** tab in **Server Settings**, click and drag this new "Bot" role to the top of the list of roles.

## 3. Setting Up the Secondary Role

- **Step 1**: Create a **Secondary Role** for the bot. This role may not have any permissions but is necessary for organizing the bot within the server.
- **Step 2**: Name this role something like "Bot Secondary" or just "Bot Role" (whatever works for your setup).
- **Step 3**: **Assign this role at the bottom of the hierarchy**.
  - Under **Server Settings** > **Roles**, drag this role to the very bottom of the role list.
  
  **Note**: The secondary role is mainly for organizing the bot's position in the **member list** on the side of Discord. It doesn't need to have permissions but can be used to place the bot **above, below, or among specific roles** (such as above the owner, below admins, or below members), depending on where you want it to show up.

## 4. Assigning Roles to the Bot

- **Step 1**: Go to your **Discord server** and click on the **Members** list.
- **Step 2**: Find your bot in the list of server members.
- **Step 3**: Right-click on the bot’s name, then click on **Roles** > Assign both the **Bot Role** (top of hierarchy) and **Secondary Role** (lowest in hierarchy).

## 5. Sorting by Hierarchy

- After assigning the roles, you need to ensure that the roles are sorted by hierarchy.
- In the **Role Settings**, under the **Roles** section, the topmost role will have the highest priority, and the lowest role will have the lowest priority. Ensure your bot’s main role is at the top.

## 6. Adjusting Permissions (if necessary)

- If your bot is not able to access certain channels or perform actions, it might be because the **bot's role** is not properly prioritized.
- Make sure no other roles with higher priority restrict access to the necessary permissions for the bot.

---

## Final Steps:

- **Test the bot**: Once the roles are set up, test the bot by asking it to perform tasks (such as sending messages or managing roles) to ensure that it has the required permissions.
- **Sort Roles**: Ensure that roles are sorted in the correct order in **Server Settings** > **Roles** tab (Bot Role at the top and Secondary Role at the bottom).

---

## Quick Recap of Hierarchy and Permissions:

- **Bot Role (Top)**: Has all permissions needed for bot operation.
- **Secondary Role (Bottom)**: Can be used for organizational purposes (it does not have any permissions), and determines the **bot’s position in the member list**.
- **Role Hierarchy**: Make sure to **sort by hierarchy** in **Server Settings** > **Roles** to keep the correct order. Place the **bot's secondary role** at the preferred position in the member list (above owner, below admin, or below members).



## Why Two Roles for the Bot?
Using two roles for your bot helps to separate its permissions from its visibility and organization within the server.

The main bot role (at the top of the hierarchy) grants all the necessary permissions the bot needs to interact with channels, manage messages, and perform its tasks.

The secondary role (at the bottom of the hierarchy) is purely for organizational purposes. It doesn’t have any permissions but determines the bot's position in the member list on the side of Discord, allowing you to control whether the bot appears above, below, or among specific roles like the owner or admins.


one last thing if u got multipel server adn want the same code/bot for it there is also a owner panel where u can hardcode ur discord id in it to execute cmd remotly annoucne leave servers u dont want the bot to be etc. 



made by TheZ
